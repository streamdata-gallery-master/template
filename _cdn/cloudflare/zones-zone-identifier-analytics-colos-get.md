---
swagger: "2.0"
info:
  title: Zone Analytics API
  description: The API for managing CloudFlare Zone Analytics
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
  /zones/:zone_identifier/analytics/colos:
    get:
      summary: This view provides a breakdown of analytics data by datacenter
      description: This view provides a breakdown of analytics data by datacenter
      operationId: cloudflare-zone-analytics-api
      parameters:
      - in: query
        name: continuous
        description: When set to true, the range returned by the response acts like
          a sliding window to provide a contiguous time-window
      - in: query
        name: since
        description: The (inclusive) beginning of the requested time frame
      - in: query
        name: until
        description: The (exclusive) end of the requested time frame
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
      - zone analytics
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