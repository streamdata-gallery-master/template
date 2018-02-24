---
swagger: "2.0"
info:
  title: AWS Security Token Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetCallerIdentity&k=1:
    get:
      summary: ' Get Caller Identity '
      description: |-
        Returns details about the IAM identity whose credentials are used to call the
              API
      operationId: getCallerIdentity
      parameters:
      - in: query
        name: Account
        description: The AWS account ID number of the account that owns or contains
          the calling      entity
        type: string
      - in: query
        name: Arn
        description: The AWS ARN associated with the calling entity
        type: string
      - in: query
        name: UserId
        description: The unique identifier of the calling entity
        type: string
      responses:
        200:
          description: OK
      tags:
      - identity
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