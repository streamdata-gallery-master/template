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
  /user/firewall/access_rules/rules:
    get:
      summary: Search, sort, and filter IP/country access rules
      description: Search, sort, and filter IP/country access rules
      operationId: cloudflare-userlevel-firewall-access-rule-api
      parameters:
      - in: query
        name: configuration_target
        description: The rule configuration targetip
      - in: query
        name: configuration_value
        description: Search by IP, range, or country code1
      - in: query
        name: direction
        description: Direction to order rulesdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)all
      - in: query
        name: mode
        description: The action to apply to a matched requestchallenge
      - in: query
        name: order
        description: Field to order rules bymode
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of rules per page50
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