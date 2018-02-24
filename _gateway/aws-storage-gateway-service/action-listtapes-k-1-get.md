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
  /?Action=ListTapes&k=1:
    get:
      summary: ' List Tapes '
      description: |-
        Lists virtual tapes in your virtual tape library (VTL) and your virtual tape shelf
                 (VTS)
      operationId: listTapes
      parameters:
      - in: query
        name: Limit
        description: An optional number limit for the tapes in the list returned by
          this call
        type: string
      - in: query
        name: Marker
        description: A string that indicates the position at which to begin the returned
          list of         tapes
        type: string
      - in: query
        name: TapeARNs
        description: The Amazon Resource Name (ARN) of each of the tapes you want
          to list
        type: string
      responses:
        200:
          description: OK
      tags:
      - tapes
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