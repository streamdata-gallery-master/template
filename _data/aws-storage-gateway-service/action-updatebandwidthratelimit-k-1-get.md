---
swagger: "2.0"
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateBandwidthRateLimit&k=1:
    get:
      summary: ' Update Bandwidth Rate Limit '
      description: Updates the bandwidth rate limits of a gateway
      operationId: updateBandwidthRateLimit
      parameters:
      - in: query
        name: AverageDownloadRateLimitInBitsPerSec
        description: The average download bandwidth rate limit in bits per second
        type: string
      - in: query
        name: AverageUploadRateLimitInBitsPerSec
        description: The average upload bandwidth rate limit in bits per second
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - bandwidth rate limit
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