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
  /?Action=DescribeAccountLimits&k=1:
    get:
      summary: ' Describe Account Limits '
      description: Retrieves your account's AWS CloudFormation limits, such as the
        maximum number of stacks that you can create in your account
      operationId: describeAccountLimits
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of limits that you want
          to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - account limits
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