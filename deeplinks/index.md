# HER Deeplinks
*   [her://](her://) Open app

## My Profile
*   [her://my_profile](her://my_profile) My Profile Page
*   [her://my_profile/edit](her://my_profile/edit) Edit Profile page
*   [her://my_profile/friends](her://my_profile/friends) My Friends Page
*   ~~[her://my_profile/preview](her://my_profile/preview)~~ My Profile Page **deprecated, needs removal from iOS**

### Questions (In Development)
*   [her://my_profile/edit/questions/1](her://my_profile/edit/questions/1) Open question with id 1
*   [her://my_profile/edit/questions](her://my_profile/edit/questions) Open questions

### Properties By Type
*   [her://my_profile/edit/properties/1](her://my_profile/edit/properties/1) Edit Height
*   [her://my_profile/edit/properties/4](her://my_profile/edit/properties/4) Edit an Identity type
*   [her://my_profile/edit/properties/5](her://my_profile/edit/properties/5) Edit Bio
*   [her://my_profile/edit/properties/10](her://my_profile/edit/properties/10) Edit a Fun Fact type
*   [her://my_profile/edit/properties/18](her://my_profile/edit/properties/18) Edit Pride Pins

### Needs implementation on Both Clients
*   [her://my_profile/events](her://my_profile/events) My Events Page
*   [her://my_profile/feed](her://my_profile/feed) My Feed Page

## User 
*   [her://user/3620800](her://user/3620800) User's Profile View
*   [her://user/3620800/friends](her://user/3620800/friends) User's Friends Page

### Needs implementation (maybe for completion's sake)
*   [her://user/3620800/feed](her://user/3620800/feed) User's Feed
*   [her://user/3620800/events](her://user/3620800/events) User's Events

## Meet
*   [her://meet](her://meet) Open Meet on Browse. (iOS) / Not supported (Android)  
*   [her://meet/likedme](her://meet/likedme) Open Meet on WLM (iOS) / Not supported (Android) 
*   [her://likedme](her://likedme) Open Meet on WLM (iOS) / Open WLM screen (Android)
*   [her://meet/online](her://meet/online) Open Meet on Online Now (iOS) / Not supported (Android) 
*   [her://onlinenow](her://onlinenow) Open Meet on Online Now (iOS) / Open Online Now (Android) 
*   [her://meet/likedme](her://meet/likedme) Open Meet on WLM (iOS) / Open WLM screen (Android)
*   [her://location](her://location) Open Meet and navigate to Change Location (iOS & Android)

## Chat
*   [her://chats](her://chats) Open Chats tab (iOS) / { Android behavior needed}
*   [her://chat/3620800](her://chat/3620800) Open Chat with user (iOS) / { Android behavior needed}
*   [her://chat_init/3620800](her://chat_init/3620800) Open Chat with user (iOS) / { Android behavior needed}
*   [her://chat_init_with_like/3620800](her://chat_init_with_like/3620800) Open Chat with user and like user (iOS) / { Android behavior needed}

## Feed
*   [her://feed/post/1](her://feed/post/1) Open post, after navigating to feed tab(iOS) / Open post details (Android)
*   [her://feed/community/20](her://feed/community/20) Open Community, after navigation to feed tab (iOS) / Open Community details (Android)
*   [her://community/20](her://community/20) Open Community, **NO** navigation to feed tab (iOS) / Not supported (Android) 
*   [her://feed/communities](her://feed/communities) Open Community list tab, after navigation to feed tab (iOS & Android)
*   [her://feed/events](her://feed/events) Open Events list tab, after navigation to feed tab (iOS) / Not supported (Android) 
*   [her://events](her://events) Open Events list tab, after navigation to feed tab (iOS) / Not supported (Android) 
*   ~~[her://ads/{id}/campaign/{id}](her://ads/{id}/campaign/{id})~~ **deprecated, needs removal from iOS**

## Notifications
*   [her://notifications](her://notifications) Open Notifications Tab
*   [her://confirm_friends](her://confirm_friends) Open's Profile.  I don't think it confirms friendship? / { Android behavior needed}

## Boosts
*   [her://boosts](her://boosts) If user has boosts open use boost page, else open purchase page (iOS) / Not supported (Android) 
    #### Query Params for her://boosts
*   [her://boosts?open=buy](her://boosts?open=buy) Open boosts purchase page regardless of number of boosts (iOS) / Not supported (Android) 
*   [her://boosts?origin_identifier=test_identifier](her://boosts) Same as her://boosts but change the origin of the purchase page (iOS) / Not supported (Android) 
*   [her://boosts?success_origin_identifier=success_test_identifier](her://boosts) Same as her://boosts but change the origin of the success / usage page (iOS) / Not supported (Android) 

Note: Any of the above URL params can be used in combination

## Premium
*   [her://premium](her://premium) Open PPP (iOS & Android)
*   [her://premium/ABCD](her://premium/ABCD) Open PPP with voucher being used (iOS & Android)
*   [her://premium/feature/11](her://premium/feature/11) Open PPP to designated feature image (iOS) / Not supported (Android)
*   ~~[her://premium/terms](her://premium/terms)~~ **deprecated, needs removal from iOS**

## Settings
*   [her://account_settings](her://account_settings) Open In-App Settings Page (iOS & Android)
*   [her://account_settings/push](her://account_settings/push) Open OS Settings App for HER (iOS & Android)
*   [her://account_settings/push_settings](her://account_settings/push_settings) Open Push Settings Page from HER Settings (iOS) / Not supported (Android) 
*   [her://account_settings/account](her://account_settings/account) Open Account Information Page from HER Settings (iOS & Android)

## General
*   ~~[her://mixher](her://mixher)~~  **deprecated, needs removal from clients**
*   [her://filters](her://filters) Open Filters for Meet(no pre-nav) / { Android behavior needed}
*   [her://verification](her://verification) Open Verification at whatever step user is at / { Android behavior needed}

## Universal links

*   [https://weareher.com/feed/posts/1241](https://weareher.com/feed/posts/1241) A feed post
*   [https://weareher.com/shared-profile?u=Z0pR9p5Ewmv3](https://weareher.com/shared-profile?u=Z0pR9p5Ewmv3) Profile in prod
*   [https://testing.weareher.com/shared-profile?u=bJO69Y19Bkvr](https://testing.weareher.com/shared-profile?u=bJO69Y19Bkvr) Profile in testing

