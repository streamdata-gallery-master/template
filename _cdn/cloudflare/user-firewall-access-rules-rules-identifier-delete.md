---
swagger: "2.0"
info:
  title: User-level Firewall access rule API
  description: The API for managing CloudFlare User-level Firewall access rule
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
  /user/firewall/access_rules/rules/:identifier:
    delete:
      summary: Remove an access rule so it is no longer evaluated during requests
      description: Remove an access rule so it is no longer evaluated during requests
      operationId: cloudflare-userlevel-firewall-access-rule-api
      responses:
        200:
          description: OK
      tags:
      - user level firewall access rule
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