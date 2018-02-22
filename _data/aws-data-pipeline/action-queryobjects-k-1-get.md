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
  /?Action=QueryObjects&k=1:
    get:
      summary: ' Query Objects '
      description: Queries the specified pipeline for the names of objects that match
        the specified set of conditions
      operationId: queryObjects
      parameters:
      - in: query
        name: limit
        description: The maximum number of object names that QueryObjects will return
          in a single call
        type: string
      - in: query
        name: marker
        description: The starting point for the results to be returned
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: query
        description: The query that defines the objects to be returned
        type: string
      - in: query
        name: sphere
        description: Indicates whether the query applies to components or instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - objects
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