---
swagger: "2.0"
info:
  title: AWS Lambda API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetPolicy&k=1:
    get:
      summary: ' Get Policy '
      description: Returns the resource policy associated with the specified Lambda
        function
      operationId: getPolicy
      parameters:
      - in: query
        name: FunctionName
        description: Function name whose resource policy you want to retrieve
        type: string
      - in: query
        name: Qualifier
        description: You can specify this optional query parameter to specify a function
          version or an alias name in which case this API will return all permissions
          associated with the specific qualified ARN
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