---
swagger: "2.0"
info:
  title: The Noun Project
  description: Icons for Everything
  version: v1
host: api.thenounproject.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user_id}/collections:
    get:
      summary: Get user collections
      description: Returns a list of collections associated with a user
      operationId: getUserCollections
      parameters:
      - in: path
        name: user_id
        description: User id
      responses:
        200:
          description: OK
      tags:
      - images
      - users
      - collections
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