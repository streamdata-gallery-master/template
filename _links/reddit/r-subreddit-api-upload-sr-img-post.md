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
  '{/r/subreddit}/api/upload_sr_img':
    post:
      summary: Add&nbsp; R Subreddit Api Upload Sr Img
      description: |-
        Add or replace a subreddit image, custom header logo, custom mobile
        icon, or custom mobile banner
      operationId: subreddits
      parameters:
      - in: query
        name: file
        description: file upload with maximum size of 500 KiB
        type: string
      - in: query
        name: formid
        description: (optional) can be ignored
        type: string
      - in: query
        name: header
        description: an integer between 0 and 1
        type: string
      - in: query
        name: img_type
        description: 'one of png or jpg (default: png)'
        type: string
      - in: query
        name: name
        description: a valid subreddit image name
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      - in: query
        name: upload_type
        description: one of (img, header, icon, banner)
        type: string
      responses:
        200:
          description: OK
      tags:
      - links
      - r
      - subreddit
      - api
      - upload
      - sr
      - img
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