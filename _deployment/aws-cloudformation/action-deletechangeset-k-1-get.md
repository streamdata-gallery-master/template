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
  /?Action=DeleteChangeSet&k=1:
    get:
      summary: ' Delete Change Set '
      description: Deletes the specified change set
      operationId: deleteChangeSet
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of the change set that
          you want to delete
        type: string
      - in: query
        name: StackName
        description: If you specified the name of a change set to delete, specify
          the stack name or ID (ARN) that is associated with it
        type: string
      responses:
        200:
          description: OK
      tags:
      - change sets
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