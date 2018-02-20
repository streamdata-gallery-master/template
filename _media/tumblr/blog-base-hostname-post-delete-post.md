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
  /blog/{base-hostname}/post/delete:
    post:
      summary: Add Blog Base Hostname Add Delete
      description: Deletes a post
      operationId: blog.base_hostname.post.delete.post
      parameters:
      - in: query
        name: id
        description: The ID of the post to delete
      responses:
        200:
          description: OK
      tags:
      - blog
      - base
      - hostname
      - post
      - delete
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