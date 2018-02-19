---
swagger: "2.0"
info:
  title: Pinterest
  description: Pinterest API
  termsOfService: https://developers.pinterest.com/terms/
  version: 1.0.0
host: api.pinterest.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me:
    get:
      summary: Get Me
      description: The default response returns the first and last name, ID and URL
        of the authenticated user
      operationId: PinterestUser
      parameters:
      - in: query
        name: fields
        description: The properties from the result objects to retrun
      responses:
        200:
          description: OK
      tags:
      - images
      - profile
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