---
swagger: "2.0"
info:
  title: Firewall access rule for a Zone API
  description: The API for managing CloudFlare Firewall access rule for a Zone
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
  /zones/:zone_id/firewall/access_rules/rules/:identifier:
    patch:
      summary: Update rule state and/or configuration for the zone
      description: Update rule state and/or configuration for the zone
      operationId: cloudflare-firewall-access-rule-for-a-zone-api
      parameters:
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: notes
        description: A personal note about the rule
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
      - firewall access rule
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