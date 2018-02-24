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
  /?Action=SetStatus&k=1:
    get:
      summary: ' Set Status '
      description: Requests that the status of the specified physical or logical pipeline
        objects be updated in the specified pipeline
      operationId: setStatus
      parameters:
      - in: query
        name: objectIds
        description: The IDs of the objects
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline that contains the objects
        type: string
      - in: query
        name: status
        description: The status to be set on all the objects specified in objectIds
        type: string
      responses:
        200:
          description: OK
      tags:
      - status
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