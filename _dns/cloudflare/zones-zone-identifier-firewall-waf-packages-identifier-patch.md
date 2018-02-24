---
swagger: "2.0"
info:
  title: WAF Rule Packages API
  description: The API for managing CloudFlare WAF Rule Packages
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
  /zones/:zone_identifier/firewall/waf/packages/:identifier:
    patch:
      summary: Change the sensitivity and action for an anomaly detection type WAF
        rule package
      description: Change the sensitivity and action for an anomaly detection type
        WAF rule package
      operationId: cloudflare-waf-rule-packages-api
      parameters:
      - in: query
        name: action_mode
        description: The default action that will be taken for rules under the firewall
          package
      - in: query
        name: sensitivity
        description: The sensitivity of the firewall package
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
      - waf rule packages
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