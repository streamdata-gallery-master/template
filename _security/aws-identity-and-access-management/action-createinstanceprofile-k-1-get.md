---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateInstanceProfile&k=1:
    get:
      summary: ' Create Instance Profile '
      description: Creates a new instance profile
      operationId: createInstanceProfile
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to create
        type: string
      - in: query
        name: Path
        description: The path to the instance profile
        type: string
      responses:
        200:
          description: OK
      tags:
      - instance profiles
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