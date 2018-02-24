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
  '{/r/subreddit}/comments/article':
    get:
      summary: Get&nbsp; R Subreddit Comments Article
      description: Get the comment tree for a given Link article
      operationId: listings
      parameters:
      - in: query
        name: article
        description: ID36 of a link
        type: string
      - in: query
        name: comment
        description: (optional) ID36 of a comment
        type: string
      - in: query
        name: context
        description: an integer between 0 and 8
        type: string
      - in: query
        name: depth
        description: (optional) an integer
        type: string
      - in: query
        name: limit
        description: (optional) an integer
        type: string
      - in: query
        name: showedits
        description: boolean value
        type: string
      - in: query
        name: showmore
        description: boolean value
        type: string
      - in: query
        name: sort
        description: one of (confidence, top, new, controversial, old, random, qa,
          live)
        type: string
      - in: query
        name: sr_detail
        description: (optional) expand subreddits
        type: string
      - in: query
        name: threaded
        description: boolean value
        type: string
      - in: query
        name: truncate
        description: an integer between 0 and 50
        type: string
      responses:
        200:
          description: OK
      tags:
      - links
      - r
      - subreddit
      - comments
      - article
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