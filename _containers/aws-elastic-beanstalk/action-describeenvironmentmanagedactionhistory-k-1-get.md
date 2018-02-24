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
  /?Action=DescribeEnvironmentManagedActionHistory&k=1:
    get:
      summary: ' Describe Environment Managed Action History '
      description: Lists an environment's completed and failed managed actions
      operationId: describeEnvironmentManagedActionHistory
      parameters:
      - in: query
        name: EnvironmentId
        description: The environment ID of the target environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the target environment
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of items to return for a single request
        type: string
      - in: query
        name: NextToken
        description: The pagination token returned by a previous request
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