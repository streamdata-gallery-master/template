---
swagger: "2.0"
info:
  title: AWS CloudHSM API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListHapgs&k=1:
    get:
      summary: ' List HAPG '
      description: Lists the high-availability partition groups for the account
      operationId: listHapgs
      parameters:
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to ListHapgs
        type: string
      responses:
        200:
          description: OK
      tags:
      - high-availability partition group
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