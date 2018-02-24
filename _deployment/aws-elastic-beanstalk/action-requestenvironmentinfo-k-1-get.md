---
swagger: "2.0"
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RequestEnvironmentInfo&k=1:
    get:
      summary: ' Request Environment Info '
      description: |-
        Initiates a request to compile the specified type of information of the deployed
              environment
      operationId: requestEnvironmentInfo
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment of the requested data
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment of the requested data
        type: string
      - in: query
        name: InfoType
        description: The type of information to request
        type: string
      responses:
        200:
          description: OK
      tags:
      - environments
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