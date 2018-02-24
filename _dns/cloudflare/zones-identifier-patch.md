---
swagger: "2.0"
info:
  title: Zone API
  description: The API for managing CloudFlare Zone
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
  /zones/:identifier:
    patch:
      summary: Only one zone property can be changed at a time
      description: Only one zone property can be changed at a time
      operationId: cloudflare-zone-api
      parameters:
      - in: query
        name: paused
        description: Indicates if the zone is only using CloudFlare DNS services
      - in: query
        name: plan
        description: The desired plan for the zone
      - in: query
        name: vanity_name_servers
        description: An array of domains used for custom name servers
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
      - zones
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