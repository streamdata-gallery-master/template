---
swagger: "2.0"
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeStep&k=1:
    get:
      summary: ' Describe Step '
      description: Provides more detail about the cluster step
      operationId: describeStep
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster with steps to describe
        type: string
      - in: query
        name: StepId
        description: The identifier of the step to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - steps
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