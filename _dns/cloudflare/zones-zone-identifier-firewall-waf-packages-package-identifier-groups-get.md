---
swagger: "2.0"
info:
  title: WAF Rule Groups API
  description: The API for managing CloudFlare WAF Rule Groups
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
  /zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups:
    get:
      summary: Search, list, and sort rule groups contained within a package
      description: Search, list, and sort rule groups contained within a package
      operationId: cloudflare-waf-rule-groups-api
      parameters:
      - in: query
        name: direction
        description: Direction to order groupsttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: mode
        description: Whether or not the rules contained within this group are configurable/usabletttttttttttttton
      - in: query
        name: name
        description: Name of the firewall rule groupttttttttttttttProject Honey Pot
      - in: query
        name: order
        description: Field to order groups byttttttttttttttmode
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of groups per pagetttttttttttttt50
      - in: query
        name: rules_count
        description: How many rules are contained within this grouptttttttttttttt10
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
      - waf rule groups
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