# HER Deeplinks

## General
- [her://](her://) — Open app

## Meet & Discover
- [her://meet](her://meet) — Open Browse (aka Meet) (iOS & Android)
- [her://meet/nearby](her://meet/nearby) — (Deprecated) Nearby (iOS & Android)
- [her://meet/likedme](her://meet/likedme) — WLM (iOS & Android) (consolidated likes in newer version)
- [her://meet/online](her://meet/online) — (Deprecated in newer versions) Online Now (iOS & Android)
- [her://meet/views](her://meet/views) — Views (iOS & Android)
- [her://nearby](her://nearby) — (Deprecated in newer versions) Nearby (iOS & Android)
- [her://likedme](her://likedme) — WLM (iOS & Android) (consolidated likes in newer version)
- [her://onlinenow](her://onlinenow) — (Deprecated in newer versions) Online Now (iOS & Android)
- [her://views](her://views) — Views (opens Discover first) (iOS & Android)
- [her://location](her://location) — Change Location (opens PPP if not premium)
- [her://filters](her://filters) — Meet Filters (no pre-nav)
- [her://meet/preset/{PRESET_ID}](her://meet/preset/{PRESET_ID}) — Meet with preset ID.  List of preset ids are near bottom of the page.

## Chat
- [her://chats](her://chats) — Chats tab
- [her://chat/{USER_ID}](her://chat/{USER_ID}) — Chat with user
- [her://chat_init/{USER_ID}](her://chat_init/{USER_ID}) — Chat with user (deprecated)
- [her://chat_init_with_like/{USER_ID}](her://chat_init_with_like/{USER_ID}) — DEPRECATED; behavior on iOS at some point changed to only send a like. 

## Feed
- [her://feed/](her://feed/) — Open post
- [her://feed/post/{POST_ID}](her://feed/post/{POST_ID}) — Open post
- [her://feed/community/{COMMUNITY_ID}](her://feed/community/{COMMUNITY_ID}) — Community
- [her://feed/communities](her://feed/communities) — Community list
- [her://feed/filters](her://feed/filters) — Feed filters
- [her://feed/events](her://feed/events) — Events list (iOS)
- [her://feed/notifications](her://feed/notifications) — Community notifications
- [her://events](her://events) — Events list
- [her://community/{COMMUNITY_ID}](her://community/{COMMUNITY_ID}) — Community.  Community IDs are listed near bottom of page.
- [her://event/{EVENT_ID}](her://event/{EVENT_ID}) — Event

## Notifications
- [her://notifications](her://notifications) — (Deprecated)Notifications (Recent Likes)
- [her://notifications/communities](her://notifications/communities) — Community notifications
- [her://notifications/likes](her://notifications/likes) — Consolidated likes

## My Profile
- [her://my_profile](her://my_profile) — My profile
- [her://my_profile/posts](her://my_profile/posts) — My posts
- [her://my_profile/feelings](her://my_profile/feelings) — Add feeling
- [her://my_profile/topartists](her://my_profile/topartists) — Spotify edit
- [her://my_profile/edit](her://my_profile/edit) — Edit profile
- [her://my_profile/edit/topartists](her://my_profile/edit/topartists) — Spotify edit
- [her://my_profile/edit/instagram](her://my_profile/edit/instagram) — Instagram edit
- [her://my_profile/edit/questions](her://my_profile/edit/questions) — Questions
- [her://my_profile/edit/questions/{QUESTION_ID}](her://my_profile/edit/questions/{QUESTION_ID}) — Question
    No chart for questions list exists on this page.  Please ask in Slack for relevat question IDs.
    
- [her://my_profile/feelings?source=SOURCE&style=STYLE](her://my_profile/feelings?source=SOURCE&style=STYLE) 
    Replace STYLE with either `halfsheet` or `fullscreen` (iOS)
    Replace SOURCE with an identifier to add to tracking data. Otherwise, `not_specified` is the source. (iOS)

### Profile Property Editing
- [her://my_profile/edit/properties/{PROPERTY_ID}](her://my_profile/edit/properties/{PROPERTY_ID}) — Append `?half=true` to show as half-sheet (iOS)


## Settings
- [her://account_settings](her://account_settings) — Settings
- [her://account_settings/push](her://account_settings/push) — OS Settings
- [her://account_settings/connected_accounts](her://account_settings/connected_accounts)
- [her://account_settings/push_settings](her://account_settings/push_settings)
- [her://account_settings/account](her://account_settings/account)
- [her://account_settings/community](her://account_settings/community)
- [her://account_settings/privacy](her://account_settings/privacy)

## Member Hub
- [her://member_hub](her://member_hub)

## User
- [her://user/{USER_ID}](her://user/{USER_ID}) — User profile
- [her://user/{USERNAME}](her://user/{USERNAME}) — Profile by username
- [her://profiles/{USERNAME}](her://profiles/{USERNAME}) — Username-only profile

## Boosts & Thirst Mode
- [her://boosts](her://boosts)
- [her://boosts/ledger](her://boosts/ledger)
- [her://boosts?open=buy](her://boosts?open=buy)
- [her://boosts?origin_identifier=ID](her://boosts?origin_identifier=ID)
Origin_identifier is tracking ID
- [her://boosts?success_origin_identifier=ID](her://boosts?success_origin_identifier=ID)
success_origin_identifier is tracking for success page 
- [her://boosts/apply?campaign_id=ID](her://boosts/apply?campaign_id=ID)



## Premium
- [her://premium](her://premium)
- [her://premium/VOUCHER](her://premium/VOUCHER) - Deprecated with HERON.  
- [her://premium/feature/{FEATURE_ID}](her://premium/feature/{FEATURE_ID})
- [her://premium/bribe](her://premium/bribe) - Deprecated with HERON

## Incentive Review
- [her://review_incentive](her://review_incentive) (Android only)

## Verification & Completion
- [her://verification](her://verification)
- [her://completion](her://completion)

## Universal Links
- https://weareher.com/shared-post/POST_ID
- https://weareher.com/shared-event/EVENT_ID
- https://share.weareher.com/shared-profile?u=USER_ID

## Property IDs

| ID | Property |
|----|----------|
| 1  | [Height](her://my_profile/edit/properties/1) |
| 2  | [Gender](her://my_profile/edit/properties/2) |
| 3  | [Relationship status](her://my_profile/edit/properties/3) |
| 4  | [Sexuality identity](her://my_profile/edit/properties/4) |
| 5  | [About](her://my_profile/edit/properties/5) |
| 6  | [Pronoun](her://my_profile/edit/properties/6) |
| 7  | [Sex](her://my_profile/edit/properties/7) |
| 8  | [Looking for](her://my_profile/edit/properties/8) |
| 9  | [Drinking](her://my_profile/edit/properties/9) |
| 10 | [Cigarettes](her://my_profile/edit/properties/10) |
| 11 | [Cannabis](her://my_profile/edit/properties1) |
| 12 | [Political views](her://my_profile/edit/properties/12) |
| 13 | [Religion](her://my_profile/edit/properties/13) |
| 14 | [Diet](her://my_profile/edit/properties/14) |
| 15 | [Star sign](her://my_profile/edit/properties/15) |
| 16 | [Pets](her://my_profile/edit/properties/16) |
| 17 | [Kids](her://my_profile/edit/properties/17) |
| 18 | [Pride pins](her://my_profile/edit/properties/18) |
| 19 | [Interests](her://my_profile/edit/properties/19) |
| 21 | [Relationship style](her://my_profile/edit/properties/21) |
| 22 | [Hometown location](her://my_profile/edit/properties/22) |
| 23 | [Resides location](her://my_profile/edit/properties/23) |
| 24 | [Relationship goal](her://my_profile/edit/properties/34) |
| 25 | [Sex](her://my_profile/edit/properties/25) |
| 26 | [Intimacy](her://my_profile/edit/properties/26) |
| 27 | [Kink](her://my_profile/edit/properties/27) |

## Communities

| ID | Community |
|----|----------|
| 8  | HERCommunity |
| 9  | Movies and TV Shows |
| 10 | Traveling and Living Abroad |
| 13 | 40+ Community |
| 15 | Mindfulness |
| 18 | Queer Women of Color |
| 19 | Trans Women |
| 23 | Artists and Musicians and Creators |
| 24 | Pro Sports and Athletes |
| 25 | Trans Man |
| 26 | Nonbinary |
| 28 | Recipes & Foodies |
| 29 | Non-monogamy |
| 30 | Coming Out Advice & Conversation |
| 31 | Lesbian |
| 32 | Bisexual |
| 33 | Thirst Trap |
| 34 | Gaming |
| 35 | Pets and Animals |
| 36 | Good Vibes Only |
| 38 | Activism and Social Justice |
| 39 | Beauty and Fashion |
| 40 | LGBTQ Parents + Families |
| 41 | In Search of Love and Dating |
| 42 | In Search of Friends |
| 43 | Body Positive and Plus Size |
| 44 | Astrology, Horoscope, etc |
| 45 | Writing and Poetry |
| 46 | Asexual |
| 47 | Music and Podcasts |

## Preset Filter IDs
- 1 Compatible Goals
- 2 Recently Online
- 3 Outdoorsy Queers
- 4 Inked Girlies
- 5 Femme
- 6 Masc
- 7 T4T
- 8 New Likes

## Store Review Links
- https://apps.apple.com/app/id573328837?action=write-review
- https://play.google.com/store/apps/details?id=com.weareher.her&showAllReviews=true
