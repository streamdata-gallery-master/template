---
swagger: "2.0"
info:
  title: AWS Batch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateJobQueue&k=1:
    get:
      summary: ' Update Job Queue '
      description: Updates a job queue
      operationId: updateJobQueue
      parameters:
      - in: query
        name: computeEnvironmentOrder
        description: Details the set of compute environments mapped to a job queue
          and their order         relative to each other
        type: string
      - in: query
        name: jobQueue
        description: The name or the Amazon Resource Name (ARN) of the job queue
        type: string
      - in: query
        name: priority
        description: The priority of the job queue
        type: string
      - in: query
        name: state
        description: Describes the queue's ability to accept new jobs
        type: string
      responses:
        200:
          description: OK
      tags:
      - job queue
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