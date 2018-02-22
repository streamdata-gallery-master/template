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
  /?Action=SetTerminationProtection&k=1:
    get:
      summary: ' Set Termination Protection '
      description: SetTerminationProtection locks a job flow so the EC2 instances
        in the cluster cannot be terminated by user intervention, an API call, or
        in the event of a job-flow error
      operationId: setTerminationProtection
      parameters:
      - in: query
        name: JobFlowIds
        description: A list of strings that uniquely identify the job flows to protect
        type: string
      - in: query
        name: TerminationProtected
        description: A Boolean that indicates whether to protect the job flow and
          prevent the Amazon EC2 instances in the cluster from shutting down due to
          API calls, user intervention, or job-flow error
        type: string
      responses:
        200:
          description: OK
      tags:
      - termination protection
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