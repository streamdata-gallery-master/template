---
swagger: "2.0"
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutConfigRule&k=1:
    get:
      summary: ' Put Config Rule '
      description: "Adds or updates an AWS Config rule for evaluating whether your
        AWS resources comply\n\t\t\twith your desired configurations"
      operationId: putConfigRule
      parameters:
      - in: query
        name: ConfigRule
        description: An AWS Config rule represents an AWS Lambda function that you
          create for a custom rule or a predefined function for an AWS managed rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - configuration rules
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