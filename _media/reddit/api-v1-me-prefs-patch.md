---
swagger: "2.0"
info:
  title: Reddit
  description: The Reddit API allows you to access the user submitted and rated stories
    on reddit.com. It also provides advanced functionality, including user account
    information and sub-reddit moderation.
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/me/prefs:
    patch:
      summary: Patch&nbsp; Api V1 Me Prefs
      description: ""
      operationId: sign-up-to-get-your-own-personalized-reddit-experience
      parameters:
      - in: query
        name: This endpoint expects JSON data of this format
        description: '{  &quot;allow_clicktracking&quot;: boolean value,  &quot;beta&quot;:
          boolean value,  &quot;clickgadget&quot;: boolean value,  &quot;collapse_read_messages&quot;:
          boolean value,  &quot;compress&quot;: boolean value,  &quot;creddit_autorenew&quot;:
          boolean value,  &quot;default_comment_sort&quot;: one of (`confidence`,
          `top`, `new`, `controversial`, `old`, `random`, `qa`, `live`),  &quot;domain_details&quot;:
          boolean value,  &quot;email_digests&quot;: boolean value,  &quot;email_messages&quot;:
          boolean value,  &quot;email_unsubscribe_all&quot;: boolean value,  &quot;enable_default_themes&quot;:
          boolean value,  &quot;g&quot;: one of (`GLOBAL`, `US`, `AR`, `AU`, `BG`,
          `CA`, `CL`, `CO`, `HR`, `CZ`, `FI`, `GR`, `HU`, `IS`, `IN`, `IE`, `JP`,
          `MY`, `MX`, `NZ`, `PH`, `PL`, `PT`, `PR`, `RO`, `RS`, `SG`, `SE`, `TW`,
          `TH`, `TR`, `GB`, `US_WA`, `US_DE`, `US_DC`, `US_WI`, `US_WV`, `US_HI`,
          `US_FL`, `US_WY`, `US_NH`, `US_NJ`, `US_NM`, `US_TX`, `US_LA`, `US_NC`,
          `US_ND`, `US_NE`, `US_TN`, `US_NY`, `US_PA`, `US_CA`, `US_NV`, `US_VA`,
          `US_CO`, `US_AK`, `US_AL`, `US_AR`, `US_VT`, `US_IL`, `US_GA`, `US_IN`,
          `US_IA`, `US_OK`, `US_AZ`, `US_ID`, `US_CT`, `US_ME`, `US_MD`, `US_MA`,
          `US_OH`, `US_UT`, `US_MO`, `US_MN`, `US_MI`, `US_RI`, `US_KS`, `US_MT`,
          `US_MS`, `US_SC`, `US_KY`, `US_OR`, `US_SD`),  &quot;hide_ads&quot;: boolean
          value,  &quot;hide_downs&quot;: boolean value,  &quot;hide_from_robots&quot;:
          boolean value,  &quot;hide_locationbar&quot;: boolean value,  &quot;hide_ups&quot;:
          boolean value,  &quot;highlight_controversial&quot;: boolean value,  &quot;highlight_new_comments&quot;:
          boolean value,  &quot;ignore_suggested_sort&quot;: boolean value,  &quot;in_redesign_beta&quot;:
          boolean value,  &quot;label_nsfw&quot;: boolean value,  &quot;lang&quot;:
          a valid IETF language tag (underscore separated),  &quot;legacy_search&quot;:
          boolean value,  &quot;live_orangereds&quot;: boolean value,  &quot;mark_messages_read&quot;:
          boolean value,  &quot;media&quot;: one of (`on`, `off`, `subreddit`),  &quot;media_preview&quot;:
          one of (`on`, `off`, `subreddit`),  &quot;min_comment_score&quot;: an integer
          between -100 and 100,  &quot;min_link_score&quot;: an integer between -100
          and 100,  &quot;monitor_mentions&quot;: boolean value,  &quot;newwindow&quot;:
          boolean value,  &quot;no_profanity&quot;: boolean value,  &quot;no_video_autoplay&quot;:
          boolean value,  &quot;num_comments&quot;: an integer between 1 and 500,  &quot;numsites&quot;:
          an integer between 1 and 100,  &quot;organic&quot;: boolean value,  &quot;other_theme&quot;:
          subreddit name,  &quot;over_18&quot;: boolean value,  &quot;private_feeds&quot;:
          boolean value,  &quot;profile_opt_out&quot;: boolean value,  &quot;public_votes&quot;:
          boolean value,  &quot;research&quot;: boolean value,  &quot;search_include_over_18&quot;:
          boolean value,  &quot;show_flair&quot;: boolean value,  &quot;show_gold_expiration&quot;:
          boolean value,  &quot;show_link_flair&quot;: boolean value,  &quot;show_promote&quot;:
          boolean value,  &quot;show_stylesheets&quot;: boolean value,  &quot;show_trending&quot;:
          boolean value,  &quot;store_visits&quot;: boolean value,  &quot;theme_selector&quot;:
          subreddit name,  &quot;threaded_messages&quot;: boolean value,  &quot;threaded_modmail&quot;:
          boolean value,  &quot;top_karma_subreddits&quot;: boolean value,  &quot;use_global_defaults&quot;:
          boolean value,}'
        type: string
      responses:
        200:
          description: OK
      tags:
      - links
      - api
      - v1
      - me
      - prefs
definitions: []
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---