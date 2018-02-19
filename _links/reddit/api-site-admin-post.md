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
  /api/site_admin:
    post:
      summary: Add&nbsp; Api Site Admin
      description: Create or configure a subreddit
      operationId: subreddits
      parameters:
      - in: query
        name: allow_discovery
        description: boolean value
        type: string
      - in: query
        name: allow_images
        description: boolean value
        type: string
      - in: query
        name: allow_post_crossposts
        description: boolean value
        type: string
      - in: query
        name: allow_top
        description: boolean value
        type: string
      - in: query
        name: allow_videos
        description: boolean value
        type: string
      - in: query
        name: api_type
        description: the string json
        type: string
      - in: query
        name: collapse_deleted_comments
        description: boolean value
        type: string
      - in: query
        name: comment_score_hide_mins
        description: 'an integer between 0 and 1440 (default: 0)'
        type: string
      - in: query
        name: description
        description: raw markdown text
        type: string
      - in: query
        name: exclude_banned_modqueue
        description: boolean value
        type: string
      - in: query
        name: free_form_reports
        description: boolean value
        type: string
      - in: query
        name: g-recaptcha-response
        type: string
      - in: query
        name: header-title
        description: a string no longer than 500 characters
        type: string
      - in: query
        name: hide_ads
        description: boolean value
        type: string
      - in: query
        name: key_color
        description: a 6-digit rgb hex color, e
        type: string
      - in: query
        name: lang
        description: a valid IETF language tag (underscore separated)
        type: string
      - in: query
        name: link_type
        description: one of (any, link, self)
        type: string
      - in: query
        name: name
        description: subreddit name
        type: string
      - in: query
        name: over_18
        description: boolean value
        type: string
      - in: query
        name: public_description
        description: raw markdown text
        type: string
      - in: query
        name: show_media
        description: boolean value
        type: string
      - in: query
        name: show_media_preview
        description: boolean value
        type: string
      - in: query
        name: spam_comments
        description: one of (low, high, all)
        type: string
      - in: query
        name: spam_links
        description: one of (low, high, all)
        type: string
      - in: query
        name: spam_selfposts
        description: one of (low, high, all)
        type: string
      - in: query
        name: spoilers_enabled
        description: boolean value
        type: string
      - in: query
        name: sr
        description: fullname of a thing
        type: string
      - in: query
        name: submit_link_label
        description: a string no longer than 60 characters
        type: string
      - in: query
        name: submit_text
        description: raw markdown text
        type: string
      - in: query
        name: submit_text_label
        description: a string no longer than 60 characters
        type: string
      - in: query
        name: suggested_comment_sort
        description: one of (confidence, top, new, controversial, old, random, qa,
          live)
        type: string
      - in: query
        name: theme_sr
        description: subreddit name
        type: string
      - in: query
        name: theme_sr_update
        description: boolean value
        type: string
      - in: query
        name: title
        description: a string no longer than 100 characters
        type: string
      - in: query
        name: type
        description: one of (gold_restricted, archived, restricted, employees_only,
          gold_only, private, user, public)
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      - in: query
        name: wikimode
        description: one of (disabled, modonly, anyone)
        type: string
      - in: query
        name: wiki_edit_age
        description: 'an integer between 0 and 36600 (default: 0)'
        type: string
      - in: query
        name: wiki_edit_karma
        description: 'an integer between 0 and 1000000000 (default: 0)'
        type: string
      responses:
        200:
          description: OK
      tags:
      - links
      - api
      - site
      - admin
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