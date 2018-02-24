---
swagger: "2.0"
info:
  title: AWS Cognito Sync API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteDataset&k=1:
    get:
      summary: ' Delete Dataset '
      description: Deletes the specific dataset
      operationId: deleteDataset
      parameters:
      - in: query
        name: DatasetName
        description: A string of up to 128 characters
        type: string
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - dataset
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