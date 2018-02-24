---
swagger: "2.0"
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutConfigurationRecorder&k=1:
    get:
      summary: ' Put Configuration Recorder '
      description: Creates a new configuration recorder to record the selected resource
        configurations
      operationId: putConfigurationRecorder
      parameters:
      - in: query
        name: ConfigurationRecorder
        description: The configuration recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - configuration recorders
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