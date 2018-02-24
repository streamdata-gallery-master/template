---
swagger: "2.0"
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GenerateRandom&k=1:
    get:
      summary: ' Generate Random '
      description: Generates an unpredictable byte string
      operationId: generateRandom
      parameters:
      - in: query
        name: NumberOfBytes
        description: The length of the byte string
        type: string
      responses:
        200:
          description: OK
      tags:
      - randoms
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