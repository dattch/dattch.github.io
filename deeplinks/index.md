# HER Deeplinks
*   [her://](her://) Open app

## Meet
*   [her://meet](her://meet) Open Meet on Browse. (iOS & Android)
*   [her://meet/nearby](her://meet/nearby) Open Meet on nearby
*   [her://meet/likedme](her://meet/likedme) Open Meet on WLM (iOS & Android) 
*   [her://meet/online](her://meet/online) Open Meet on Online Now (iOS) / Opens Online Now swiping screen (Android) 
*   [her://nearby](her://nearby) Open Meet on nearby, iOS only
*   [her://likedme](her://likedme) Open Meet on WLM (iOS) / Open WLM screen (Android)
*   [her://onlinenow](her://onlinenow) Open Meet on Online Now (iOS) / Open Online Now (Android) 
*   [her://location](her://location) Open Meet and navigate to Change Location (iOS & Android).  Opens PPP if not a premium user.
*   [her://filters](her://filters) Open Filters for Meet(no pre-nav) (iOS & Android)

## Chat
*   [her://chats](her://chats) Open Chats tab (iOS & Android)
*   [her://chat/3620800](her://chat/3620800) Open Chat with user  (iOS & Android)
*   [her://chat_init/3620800](her://chat_init/3620800) Open Chat with user  (iOS & Android) (should be deprecated?)
*   [her://chat_init_with_like/3620800](her://chat_init_with_like/3620800) Open Chat with user and like user (iOS & Android)

## Feed
*   [her://feed/](her://feed/) Open post, after navigating to feed tab(iOS) / Open post details (Android)
*   [her://feed/post/1](her://feed/post/1) Open post, after navigating to feed tab(iOS) / Open post details (Android)
*   [her://feed/community/20](her://feed/community/44) Open Community, after navigation to feed tab (iOS) / Open Community details (Android)
*   [her://feed/communities](her://feed/communities) Open Community list tab, after navigation to feed tab (iOS & Android)
*   [her://feed/filters](her://feed/filters) Open Feed filters, after navigation to feed tab (iOS & Android)
*   [her://feed/events](her://feed/events) Open Events list tab, after navigation to feed tab (iOS) / Not supported (Android) 
*   [her://events](her://events) Open Events list tab, after navigation to feed tab (iOS - **needs update to not navigate to feed**) / Not supported (Android) 
*   [her://community/44](her://community/44) Open Community, **NO** navigation to feed tab (iOS) / Not supported (Android) 
*   [her://event/353](her://event/353) Open Event, direct navigation (iOS) / Not supported (Android) 

## Notifications
*   [her://notifications](her://notifications) Open Notifications Tab
*   [her://notifications/likes/3620800](her://notifications/likes/3620800) Open Notifications Tab, on the likes sub tab, with user id 3620800 first to appear if that user has liked your profile.  
*   [her://notifications/likes/ZVm2XpL7G235](her://notifications/likes/ZVm2XpL7G235) Open Notifications Tab, on the likes sub tab, with user id ZVm2XpL7G235 first to appear if that user has liked your profile.  
*   [her://notifications/matches](her://notifications/matches) Open Notifications Tab, on the matches sub tab
*   [her://notifications/communities](her://notifications/communities) Open Notifications Tab, on the communities sub tab
*   [her://confirm_friend/3620800](her://confirm_friend/3620800) Opens Profile with ID 3620800 and triggers a request to the /friends endpoint to confirm friend request. (iOS & Android) (Broken on iOS pre-6.15.2, only works from notifications page successfully)
*   
## My Profile
*   [her://my_profile](her://my_profile) My Profile Page
*   [her://my_profile/friends](her://my_profile/friends) My Friends Page
*   [her://my_profile/posts](her://my_profile/posts) My feed posts Page
*   [her://my_profile/topartists](her://my_profile/topartists) Open edit page and scroll to spotify section
*   [her://my_profile/edit](her://my_profile/edit) Edit Profile page
*   [her://my_profile/edit/topartists](her://my_profile/edit/topartists) Open edit page and scroll to spotify section
*   [her://my_profile/edit/instagram](her://my_profile/edit/instagram) Open edit page and scroll to instagram section
*   [her://my_profile/edit/questions](her://my_profile/edit/questions) Open questions page
*   [her://my_profile/edit/questions/17](her://my_profile/edit/questions/17) Open question with id 17
To edit a profile property, we need to find out the ID for that property and link to `her://my_profile/edit/properties/{property_id}`. Some examples:
*   [her://my_profile/edit/properties/1](her://my_profile/edit/properties/1) Edit Height
*   [her://my_profile/edit/properties/4](her://my_profile/edit/properties/4) Edit an Identity type
*   [her://my_profile/edit/properties/5](her://my_profile/edit/properties/5) Edit Bio
*   [her://my_profile/edit/properties/10](her://my_profile/edit/properties/10) Edit a Fun Fact type
*   [her://my_profile/edit/properties/18](her://my_profile/edit/properties/18) Edit Pride Pins

## Settings
*   [her://account_settings](her://account_settings) Open In-App Settings Page (iOS & Android)
*   [her://account_settings/push](her://account_settings/push) Open OS Settings App for HER (iOS & Android)
*   [her://account_settings/push_settings](her://account_settings/push_settings) Open Push Settings Page from HER Settings (iOS) / Open OS Settings App for HER (Android) 
*   [her://account_settings/account](her://account_settings/account) Open Account Information Page from HER Settings (iOS & Android)
*   [her://account_settings/community] (her://account_settings/community) Open community subscription if user is not subscribed or if otherwise open manange subscriptions settings (iOS)

## User 
*   [her://user/3620800](her://user/3620800) User's Profile View
*   [her://user/3620800/friends](her://user/3620800/friends) User's Friends Page
Note: alternatively, use username instead of user id, such as [her://user/ZVm2XpL7G235](her://user/ZVm2XpL7G235)
Note 2: Alt format that supports only username is [her://profiles/ZVm2XpL7G235](her://profiles/ZVm2XpL7G235)

## Boosts
*   [her://boosts](her://boosts) If user has boosts open use boost page, else open purchase page (iOS & Android) 
    #### Query Params for her://boosts
*   [her://boosts?open=buy](her://boosts?open=buy) Open boosts purchase page regardless of number of boosts (iOS) / open boost purchase page (Android) 
*   [her://boosts?origin_identifier=test_identifier](her://boosts) Same as her://boosts but change the origin of the purchase page (iOS & Android) 
*   [her://boosts?success_origin_identifier=success_test_identifier](her://boosts) Same as her://boosts but change the origin of the success / usage page (iOS) / open boost purchase page (Android) 

Note: Any of the above URL params can be used in combination

## Premium
*   [her://premium](her://premium) Open PPP (iOS & Android)
*   [her://premium/ABCD](her://premium/ABCD) Open PPP with voucher being used (iOS & Android)
*   [her://premium/feature/11](her://premium/feature/11) Open PPP to designated feature image (iOS) / Not supported (Android)
*   [her://premium/bribe](her://premium/bribe) Open PPP to 24 bribe for review (iOS) / Not supported (Android)

## General
*   [her://verification](her://verification) Open Verification at whatever step user is at (iOS & Android)
*   [her://completion](her://completion) Opens the Profile completion flow

## Universal links

*   [https://weareher.com/shared-post/1241](https://weareher.com/shared-post/1241) A feed post
*   [https://weareher.com/shared-event/344](https://weareher.com/shared-event/1241) An even link
*   [https://share.weareher.com/shared-profile?u=Z0pR9p5Ewmv3](https://weareher.com/shared-profile?u=Z0pR9p5Ewmv3) Profile

Note: if in the test environment, links generated by the application might use subdomain `testing.` or `testshare.`
Note: Profiles were moved to the new share subdomain, events and posts have not yet.
