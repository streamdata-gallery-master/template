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
  /blog/{base-hostname}/post/edit:
    post:
      summary: Add Blog Base Hostname Add Edit
      description: Edits a blog post
      operationId: blog.base_hostname.post.edit.post
      parameters:
      - in: query
        name: date
        description: The GMT date and time of the post, as a string
      - in: query
        name: id
        description: The ID of the post to edit
      - in: query
        name: markdown
        description: Indicates whether the post uses markdown syntax
      - in: query
        name: tags
        description: Comma-separated tags for this post
      - in: query
        name: tweet
        description: 'Manages the autotweet (if enabled) for this post: set to off
          for no tweet, or enter text to override the default tweet'
      - in: query
        name: type
        description: The post type
      responses:
        200:
          description: OK
      tags:
      - blog
      - base
      - hostname
      - post
      - edit
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