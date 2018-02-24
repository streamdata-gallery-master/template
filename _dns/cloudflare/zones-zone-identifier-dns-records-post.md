---
swagger: "2.0"
info:
  title: DNS Records for a Zone API
  description: The API for managing CloudFlare DNS Records for a Zone
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
  /zones/:zone_identifier/dns_records:
    post:
      summary: Create a new DNS record for a zone
      description: Create a new DNS record for a zone
      operationId: cloudflare-dns-records-for-a-zone-api
      parameters:
      - in: query
        name: content
        description: DNS record contenttttttttttttttt127
      - in: query
        name: name
        description: DNS record namettttttttttttttexample
      - in: query
        name: type
        description: DNS record typettttttttttttttA
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
      - records
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