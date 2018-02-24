---
swagger: "2.0"
info:
  title: Keyless SSL for a Zone API
  description: The API for managing CloudFlare Keyless SSL for a Zone
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
  /zones/:zone_identifier/keyless_certificates/:identifier:
    get:
      summary: Details for one Keyless SSL configuration
      description: Details for one Keyless SSL configuration
      operationId: cloudflare-keyless-ssl-for-a-zone-api
      responses:
        200:
          description: OK
      tags:
      - keyless certificates
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