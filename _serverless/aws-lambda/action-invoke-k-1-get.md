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
  /?Action=Invoke&k=1:
    get:
      summary: ' Invoke '
      description: Invokes a specific Lambda function
      operationId: invoke
      parameters:
      - in: query
        name: ClientContext
        description: Using the ClientContext you can pass client-specific information
          to the       Lambda function you are invoking
        type: string
      - in: query
        name: FunctionName
        description: The Lambda function name
        type: string
      - in: query
        name: InvocationType
        description: By default, the Invoke API assumes RequestResponse invocation
          type
        type: string
      - in: query
        name: LogType
        description: You can set this optional parameter to Tail in the request only       if
          you specify the InvocationType parameter with value RequestResponse
        type: string
      - in: query
        name: Qualifier
        description: You can use this optional parameter to specify a Lambda function
          version or alias name
        type: string
      responses:
        200:
          description: OK
      tags:
      - invoke
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