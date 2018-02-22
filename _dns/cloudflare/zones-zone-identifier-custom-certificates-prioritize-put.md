---
swagger: "2.0"
info:
  title: Custom SSL for a Zone API
  description: The API for managing CloudFlare Custom SSL for a Zone
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
  /zones/:zone_identifier/custom_certificates/prioritize:
    put:
      summary: If a zone has multiple SSL certificates, you can set the order in which
        they should be used during a request
      description: If a zone has multiple SSL certificates, you can set the order
        in which they should be used during a request
      operationId: cloudflare-custom-ssl-for-a-zone-api
      parameters:
      - in: query
        name: certificates
        description: Array of ordered certificates
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
      - certificates
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