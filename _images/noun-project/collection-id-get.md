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
  /collection/{id}:
    get:
      summary: Get collection by id
      description: Returns a single collection
      operationId: getCollectionById
      parameters:
      - in: path
        name: id
        description: Collection id
      responses:
        200:
          description: OK
      tags:
      - images
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