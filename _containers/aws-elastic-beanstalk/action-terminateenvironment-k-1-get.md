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
  /?Action=TerminateEnvironment&k=1:
    get:
      summary: ' Terminate Environment '
      description: Terminates the specified environment
      operationId: terminateEnvironment
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to terminate
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to terminate
        type: string
      - in: query
        name: ForceTerminate
        description: Terminates the target environment even if another environment
          in the same group is      dependent on it
        type: string
      - in: query
        name: TerminateResources
        description: 'Indicates whether the associated AWS resources should shut down
          when the environment is      terminated:'
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