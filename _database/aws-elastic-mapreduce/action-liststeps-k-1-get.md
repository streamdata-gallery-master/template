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
  /?Action=ListSteps&k=1:
    get:
      summary: ' List Steps '
      description: Provides a list of steps for the cluster in reverse order unless
        you specify stepIds with the request
      operationId: listSteps
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster for which to list the steps
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      - in: query
        name: StepIds
        description: The filter to limit the step list based on the identifier of
          the steps
        type: string
      - in: query
        name: StepStates
        description: The filter to limit the step list based on certain states
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