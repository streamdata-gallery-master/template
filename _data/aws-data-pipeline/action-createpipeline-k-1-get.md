---
swagger: "2.0"
info:
  title: AWS Data Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreatePipeline&k=1:
    get:
      summary: ' Create Pipeline '
      description: Creates a new, empty pipeline
      operationId: createPipeline
      parameters:
      - in: query
        name: description
        description: The description for the pipeline
        type: string
      - in: query
        name: name
        description: The name for the pipeline
        type: string
      - in: query
        name: tags
        description: A list of tags to associate with the pipeline at creation
        type: string
      - in: query
        name: uniqueId
        description: A unique identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - pipeline
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