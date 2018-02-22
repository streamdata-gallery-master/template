---
swagger: "2.0"
info:
  title: Railgun API
  description: The API for managing CloudFlare Railgun
  termsOfService: https://www.cloudflare.com/terms/
  version: 1.0.0
host: api.cloudflare.com
basePath: /client/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /railguns/:identifier:
    patch:
      summary: Enable or disable a Railgun for all zones connected to it
      description: Enable or disable a Railgun for all zones connected to it
      operationId: cloudflare-railgun-api
      parameters:
      - in: query
        name: enabled
        description: Flag to determine if the Railgun is accepting connectionstttttttttttttttrue
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - performance
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