---
swagger: "2.0"
info:
  title: AWS Snowball API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetSnowballUsage&k=1:
    get:
      summary: ' Get Snowball Usage '
      description: |-
        Returns information about the Snowball service limit for your account, and also the
              number of Snowballs your account has in use
      operationId: getSnowballUsage
      parameters:
      - in: query
        name: SnowballLimit
        description: The service limit for number of Snowballs this account can have
          at once
        type: string
      - in: query
        name: SnowballsInUse
        description: The number of Snowballs that this account is currently using
        type: string
      responses:
        200:
          description: OK
      tags:
      - usage
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