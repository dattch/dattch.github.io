## Handling a Deeplink

1) Honor the components sequentially.  
Example: `her://feed/communities` will first open up the "feed" and then open up the "communities"
2) We should strive for url component indepenence as much as possible. 
    - Example: `her://feed/verification` vs `her://my_profile/verification` vs `her://verification`
    - Respectively: navigate to feed then check verification; navigation to my profile then check verification; regular app launch and the check verification.
    - Second note:  This will result in some dependent cases having the same behaviors.  One such example is from rule 1.  `her://feed/communities` and `her://communities` should actually have the same behavior at the time being, as communities list is presently dependent on feed.  However, this may not always be the case in the future and we should be mindful of that.
    - Note: this may be hard to achieve for the time being but I believe with a bit of work we can make this be true in most cases.
3) Any integer value path component is obviously paired to the path compenent beforehand. 
    - Example: `her://community/9` or `her://feed/community/9`.  The first will open up the app normally
    - Older example: `her://feed/ads/12/campaign_id/5`.  Back when we supported this ad system, we accepted either `her://feed/ads/12/campaign_id/5` or `her://feed/ads/12/5` as the same thing.  Cases like the latter should be considered malformed and we should ultimate result in opening the first component only, "feed".
4) URL query params should be paired with the every compatible component
    - Very few components presently use query params.  I believe the full list is here:
        - `premium` : query param `key` can be used to change the PPP origin for open, selected, and bought track events.
        - `location`: query param `origin` can be used to change the origin for track events related to change location page.
        - `boosts`: query param `origin_identifier` will change the tracking origin for the boost purchase page, `success_origin_identifier` will change tracking origin for the usage / puchase success page(defaults to value of `origin_identifier` if not set), and `open=buy` can override the default behavior to always open the purchase page even when there are boosts available. 
        Note: In the above cases `key`, `origin`, and `origin_identifier` could have been named the same seeing as they have the same relative behavior. Let's say `origin` was used.  If that had been true, if a deeplink scheme came up that was `her://location/premium?origin=testing` then it should work for both.
5) Modal Navigation won't be honored
    - Some items, such as `premium` and `verification` are modals.  In HER iOS architecure, typically this means the modal has no awareness of the navigation stack as all the modals designed in the app to date have no navigation bar implemented.  Without a navigation stack, no further View Controllers can be presented.  There are ways of re-implementing modals such that they can have a navigation stack without a navigation bar, however, most of the modals to date are things we wouldn't want to add navigation on top of typically and the work to do so could be quite a lot depending on how many modals we presently have within the application that can be deeplinked to.  Besides, I believe further navigation attempts won't be honored by the OS anyways in this context until implementation.
6) Naively handle multiple components that are all tab bar items
- Example: `her://feed/my_profile`  ... These are both tab bar components, so yes, first the handler should "select" the feed tab, and then it should select the `profile` tab. 
7) Lower case everything before processing. Deeplinks should not be case sensitive.
7) Outstanding questions:
    - Given the above rules, how would `her://feed/community/9` work?  Should it open the community feed right over the main feed or should it open feed, tab over to `communities` and then open the community feed? If former, then does that mean `her://feed/communities/community/9` would be the new link to have the app navigate to that tab before opening the community feed for 9?
        
## Designing a Deeplink

1) Use plural nouns for resource descriptions, singular for all else.
Let's talk some bad deeplink designs that exist presently or existed in the past:
`her://feed/community/9` and `her://feed/communities` .  `community` should have been implemented as plural `communities`. `her://feed/post/23423` is the same way and should be `her://feed/posts/23423`
2) Never use hyphens/underscores/etc in path compenents.
3) Use query params only for complex parameterization.  A bad example is `her://boosts?open=buy` which is a current valid deeplink.  Instead, it could have simply been `her://boosts/purchase` .  If using a query param and it has the same relative functionality as one for a different url component, use the same name for complimentary functionality.  Bad example:  `key`, `origin`, and `origin_identifier` all have the same functionality but for different url components. 
4) Keep into consideration the handling deeplink rules in the previous section

