---
swagger: "2.0"
info:
  title: AWS CloudSearch Configuration API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DefineExpression&k=1:
    get:
      summary: Define Expression
      description: Configures an Expression  for the search domain
      operationId: DefineExpression
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: Expression
        description: A named expression that can be evaluated at search time
        type: string
      responses:
        200:
          description: OK
      tags:
      - expressions
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