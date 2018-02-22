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
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET/responses/200:
    get:
      summary: Get Response
      description: Represents a method response of a given HTTP status code returned
        to the client
      operationId: methodResponse
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: responseModels
        description: Specifies the Model resources used for the response&#39;s content-type
        type: string
      - in: query
        name: responseParameters
        description: A key-value map specifying required or optional response parameters
          that Amazon API Gateway can send back to the caller
        type: string
      - in: query
        name: statusCode
        description: The method response&#39;s status code
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - api method response
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