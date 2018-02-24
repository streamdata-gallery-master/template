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
  /?Action=DescribeTapeArchives&k=1:
    get:
      summary: ' Describe Tape Archives '
      description: |-
        Returns a description of specified virtual tapes in the virtual tape shelf
                 (VTS)
      operationId: describeTapeArchives
      parameters:
      - in: query
        name: Limit
        description: Specifies that the number of virtual tapes descried be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing virtual         tapes
        type: string
      - in: query
        name: TapeARNs
        description: Specifies one or more unique Amazon Resource Names (ARNs) that
          represent the virtual         tapes you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - tape archives
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