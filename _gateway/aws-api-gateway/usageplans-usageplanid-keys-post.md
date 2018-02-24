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
  usageplans/{usageplanId}/keys:
    post:
      summary: Usageplankey Create
      description: Creates a UsagePlanKey resource to associate an existing API key
        to the specified usage plan
      operationId: usageplankeyCreate
      parameters:
      - in: body
        name: apiId
        description: API Id of the associated API stage in a usage plan
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: AttributeName.N
        description: One or more account attribute names
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: method
        description: The HTTP verb of a method
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: name
        description: The name of the targeted API entity
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: stage
        description: API stage name of the associated API stage in a usage plan
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: statusCode
        description: The HTTP status code of a response
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: type
        description: The type of API entity to which the documentation content applies
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - keys
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