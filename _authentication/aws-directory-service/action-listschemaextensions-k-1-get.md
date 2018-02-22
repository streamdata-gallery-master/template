---
swagger: "2.0"
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListSchemaExtensions&k=1:
    get:
      summary: ' List Schema Extensions '
      description: Lists all schema extensions applied to a Microsoft AD Directory
      operationId: listSchemaExtensions
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory from which to retrieve the schema
          extension information
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return
        type: string
      - in: query
        name: NextToken
        description: The ListSchemaExtensions
        type: string
      responses:
        200:
          description: OK
      tags:
      - schema extension
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