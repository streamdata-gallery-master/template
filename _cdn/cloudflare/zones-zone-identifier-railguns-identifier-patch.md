---
swagger: "2.0"
info:
  title: Railgun connections for a Zone API
  description: The API for managing CloudFlare Railgun connections for a Zone
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
  /zones/:zone_identifier/railguns/:identifier:
    patch:
      summary: Connect or disconnect a Railgun
      description: Connect or disconnect a Railgun
      operationId: cloudflare-railgun-connections-for-a-zone-api
      parameters:
      - in: query
        name: connected
        description: A flag indicating whether the given zone is connected to the
          Railguntttttttttttttttrue
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