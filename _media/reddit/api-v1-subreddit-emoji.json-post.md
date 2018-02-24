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
  /api/v1/subreddit/emoji.json:
    post:
      summary: Add&nbsp; Api V1 Subreddit Emoji.json
      description: Add an emoji to the DB by posting a message on emoji_upload_q
      operationId: emoji
      parameters:
      - in: query
        name: name
        description: Name of the emoji to be created
        type: string
      - in: query
        name: s3_key
        description: S3 key of the uploaded image which can be obtained from the S3
          url
        type: string
      responses:
        200:
          description: OK
      tags:
      - links
      - api
      - v1
      - subreddit
      - emoji.json
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