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
  '{/r/subreddit}/sticky':
    get:
      summary: Get&nbsp; R Subreddit Sticky
      description: Redirect to one of the posts stickied in the current subreddit
      operationId: subreddits
      parameters:
      - in: query
        name: num
        description: 'an integer between 1 and 2 (default: 1)'
        type: string
      responses:
        200:
          description: OK
      tags:
      - links
      - r
      - subreddit
      - sticky
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