---
swagger: "2.0"
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ContinueUpdateRollback&k=1:
    get:
      summary: ' Continue Update Rollback '
      description: |-
        For a specified stack that is in the UPDATE_ROLLBACK_FAILED state, continues rolling it back
                 to the UPDATE_ROLLBACK_COMPLETE state
      operationId: continueUpdateRollback
      parameters:
      - in: query
        name: ResourcesToSkip.member.N
        description: A list of the logical IDs of the resources that AWS CloudFormation
          skips during the continue update rollback operation
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to roll back
          the stack
        type: string
      - in: query
        name: StackName
        description: The name or the unique ID of the stack that you want to continue
          rolling back
        type: string
      responses:
        200:
          description: OK
      tags:
      - rollback
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