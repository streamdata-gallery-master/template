---
swagger: "2.0"
info:
  title: Zone API
  description: The API for managing CloudFlare Zone
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
  /zones/:identifier/purge_cache:
    delete:
      summary: Remove ALL files from CloudFlare&#39;s cache
      description: Remove ALL files from CloudFlare&#39;s cache
      operationId: cloudflare-zone-api
      parameters:
      - in: query
        name: files
        description: An array of URLs that should be removed from cachetttttttttttttt[http://www
      - in: query
        name: purge_everything
        description: A flag that indicates all resources in CloudFlares cache should
          be removed
      - in: query
        name: tags
        description: Any assets served with a Cache-Tag header that matches one of
          the provided values will be purged from the CloudFlare cachetttttttttttttt[some-tag,another-tag]
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
      - zones
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