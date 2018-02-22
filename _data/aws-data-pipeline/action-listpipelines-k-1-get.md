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
  /?Action=ListPipelines&k=1:
    get:
      summary: ' List Pipelines '
      description: Lists the pipeline identifiers for all active pipelines that you
        have permission to access
      operationId: listPipelines
      parameters:
      - in: query
        name: marker
        description: The starting point for the results to be returned
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