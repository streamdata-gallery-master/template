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
  /?Action=RebuildEnvironment&k=1:
    get:
      summary: ' Rebuild Environment '
      description: |-
        Deletes and recreates all of the AWS resources (for example: the Auto Scaling group,
              load balancer, etc
      operationId: rebuildEnvironment
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to rebuild
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to rebuild
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