---
swagger: "2.0"
info:
  title: AWS DynamoDB API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTable&k=1:
    get:
      summary: ' Describe Table '
      description: Returns information about the table, including the current status
        of the table, when it was created, the primary key schema, and any indexes
        on the table
      operationId: describeTable
      parameters:
      - in: query
        name: TableName
        description: The name of the table to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - tables
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