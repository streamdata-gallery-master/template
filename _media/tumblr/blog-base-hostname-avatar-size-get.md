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
  /blog/{base-hostname}/avatar/{size}:
    get:
      summary: Get Blog Base Hostname Avatar Size
      description: Retrieves a blog's avatar in one of 9 different sizes
      operationId: blog.base_hostname.avatar.size.get
      responses:
        200:
          description: OK
      tags:
      - blog
      - base
      - hostname
      - avatar
      - size
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