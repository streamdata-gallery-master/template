---
swagger: "2.0"
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetResourceConfigHistory&k=1:
    get:
      summary: ' Get Resource Config History '
      description: Returns a list of configuration items for the specified resource
      operationId: getResourceConfigHistory
      parameters:
      - in: query
        name: chronologicalOrder
        description: The chronological order for configuration items listed
        type: string
      - in: query
        name: earlierTime
        description: The time stamp that indicates an earlier time
        type: string
      - in: query
        name: laterTime
        description: The time stamp that indicates a later time
        type: string
      - in: query
        name: limit
        description: The maximum number of configuration items returned on each page
        type: string
      - in: query
        name: nextToken
        description: "The nextToken string returned on a previous page that\t\t\tyou
          use to get the next page of results in a paginated response"
        type: string
      - in: query
        name: resourceId
        description: The ID of the resource (for example
        type: string
      - in: query
        name: resourceType
        description: The resource type
        type: string
      responses:
        200:
          description: OK
      tags:
      - resource configurations
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