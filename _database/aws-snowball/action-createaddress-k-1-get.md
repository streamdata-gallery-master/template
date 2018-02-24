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
  /?Action=CreateAddress&k=1:
    get:
      summary: ' Create Address '
      description: Creates an address for a Snowball to be shipped to
      operationId: createAddress
      parameters:
      - in: query
        name: Address
        description: The address that you want the Snowball shipped to
        type: string
      responses:
        200:
          description: OK
      tags:
      - addresses
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