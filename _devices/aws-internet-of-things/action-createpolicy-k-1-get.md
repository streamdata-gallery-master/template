---
swagger: "2.0"
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreatePolicy&k=1:
    get:
      summary: ' Create Policy '
      description: Creates an AWS IoT policy
      operationId: createPolicy
      parameters:
      - in: query
        name: policyDocument
        description: The JSON document that describes the policy
        type: string
      - in: query
        name: policyName
        description: The policy name
        type: string
      responses:
        200:
          description: OK
      tags:
      - policies
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