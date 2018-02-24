---
swagger: "2.0"
info:
  title: Users Invites API
  description: The API for managing CloudFlare User&amp;#x27;s Invites
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
  /user/invites/:identifier:
    get:
      summary: Get the details of an invitation
      description: Get the details of an invitation
      operationId: cloudflare-userx27s-invites-api
      responses:
        200:
          description: OK
      tags:
      - user invites
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