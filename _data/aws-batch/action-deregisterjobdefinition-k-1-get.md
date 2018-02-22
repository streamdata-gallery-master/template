---
swagger: "2.0"
info:
  title: AWS Batch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeregisterJobDefinition&k=1:
    get:
      summary: ' Deregister Job Definition '
      description: Deregisters an AWS Batch job definition
      operationId: deregisterJobDefinition
      parameters:
      - in: query
        name: jobDefinition
        description: The name and revision (name:revision) or full Amazon Resource
          Name (ARN) of the job         definition to deregister
        type: string
      responses:
        200:
          description: OK
      tags:
      - job definitions
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