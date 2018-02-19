---
swagger: "2.0"
info:
  title: Tumblr
  description: "\tShare photos, mobile apps, and social network using Tumblr's API's.
    \   "
  version: 1.0.0
host: api.tumblr.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blog/{base-hostname}/posts/{type}:
    get:
      summary: Get Blog Base Hostname Adds Type
      description: Retrieves published posts
      operationId: blog.base_hostname.posts.type.get
      parameters:
      - in: query
        name: format
        description: Specifies the post format to return, other than HTML
      - in: query
        name: id
        description: A specific post ID
      - in: query
        name: limit
        description: "The number of posts to return: 1\u201320, inclusive"
      - in: query
        name: notes_info
        description: Indicates whether to return notes information (specify true or
          false)
      - in: query
        name: offset
        description: Post number to start at
      - in: query
        name: reblog_info
        description: Indicates whether to return reblog information (specify true
          or false)
      - in: query
        name: tag
        description: Limits the response to posts with the specified tag
      responses:
        200:
          description: OK
      tags:
      - blog
      - base
      - hostname
      - posts
      - type
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