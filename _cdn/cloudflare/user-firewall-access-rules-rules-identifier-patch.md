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
    patch:
      summary: Update rule state and/or configuration
      description: Update rule state and/or configuration
      operationId: cloudflare-userlevel-firewall-access-rule-api
      parameters:
      - in: query
        name: configuration
        description: Rule configurationOne of the following:Show definition &raquo;Name
          /typeDescription /exampleConstraintstargetstring
      - in: query
        name: mode
        description: The action to apply to a matched requestchallenge
      - in: query
        name: value
        description: The IP address to target in requests1
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