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
  /?Action=CancelSteps&k=1:
    get:
      summary: ' Cancel Steps '
      description: Cancels a pending step or steps in a running cluster
      operationId: cancelSteps
      parameters:
      - in: query
        name: ClusterId
        description: The ClusterID for which specified steps will be canceled
        type: string
      - in: query
        name: StepIds
        description: The list of StepIDs to cancel
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