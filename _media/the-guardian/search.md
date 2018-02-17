---
swagger: "2.0"
info:
  title: The Guardian
  description: The Guardian Content API is a public service for accessing all the
    content the Guardian creates and the collections we have of that content (tags
    and sections). There are over one and a half million items available published
    as far back as 1999. This overview will give you some idea of what data is available,
    how to find what you need, and what you will see when you make a request to us.
  version: v1
host: content.guardianapis.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Search
      description: Searches news content across the Guardian news platform
      operationId: search
      responses:
        200:
          description: OK
      tags:
      - news
definitions: []
x-streamrank:
  polling_total_time_average: ~
  polling_size_download_average: ~
  streaming_total_time_average: ~
  streaming_size_download_average: ~
  change_yes: ~
  change_no: ~
  time_percentage: ~
  size_percentage: ~
  change_percentage: ~
  last_run: ~
  days_run: ~
  minute_run: ~
---