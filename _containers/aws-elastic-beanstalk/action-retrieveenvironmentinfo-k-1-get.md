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
  /?Action=RetrieveEnvironmentInfo&k=1:
    get:
      summary: ' Retrieve Environment Info '
      description: Retrieves the compiled information from a
      operationId: retrieveEnvironmentInfo
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the data's environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the data's environment
        type: string
      - in: query
        name: InfoType
        description: The type of information to retrieve
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