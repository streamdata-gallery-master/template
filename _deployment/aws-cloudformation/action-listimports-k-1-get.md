---
swagger: "2.0"
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListImports&k=1:
    get:
      summary: ' List Imports '
      description: Lists all stacks that are importing an exported output value
      operationId: listImports
      parameters:
      - in: query
        name: ExportName
        description: The name of the exported output value
        type: string
      - in: query
        name: NextToken
        description: A string (provided by the ListImports response output) that         identifies
          the next page of stacks that are importing the specified exported output
          value
        type: string
      responses:
        200:
          description: OK
      tags:
      - imports
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