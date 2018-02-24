---
swagger: "2.0"
info:
  title: AWS API Gateway API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  is:
    authorizationtype</code>:
      summary: Method Put
      description: Create a Method resource on a specified Resource resource
      operationId: methodPut
      parameters:
      - in: header
        name: '&quot;authorizationType&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ProductCode
        description: The product code
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
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