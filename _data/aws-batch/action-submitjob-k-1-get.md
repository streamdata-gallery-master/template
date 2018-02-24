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
  /?Action=SubmitJob&k=1:
    get:
      summary: ' Submit Job '
      description: Submits an AWS Batch job from a job definition
      operationId: submitJob
      parameters:
      - in: query
        name: containerOverrides
        description: A list of container overrides in JSON format that specify the
          name of a container in         the specified job definition and the overrides
          it should receive
        type: string
      - in: query
        name: dependsOn
        description: A list of job names or IDs on which this job depends
        type: string
      - in: query
        name: jobDefinition
        description: The job definition used by this job
        type: string
      - in: query
        name: jobName
        description: The name of the job
        type: string
      - in: query
        name: jobQueue
        description: The job queue into which the job will be submitted
        type: string
      - in: query
        name: parameters
        description: Additional parameters passed to the job that replace parameter
          substitution         placeholders that are set in the job definition
        type: string
      responses:
        200:
          description: OK
      tags:
      - jobs
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