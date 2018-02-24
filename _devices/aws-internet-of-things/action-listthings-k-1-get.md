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
  /?Action=ListThings&k=1:
    get:
      summary: ' List Things '
      description: Lists your things
      operationId: listThings
      parameters:
      - in: query
        name: attributeName
        description: The attribute name used to search for things
        type: string
      - in: query
        name: attributeValue
        description: The attribute value used to search for things
        type: string
      - in: query
        name: maxResults
        description: The maximum number of results to return in this operation
        type: string
      - in: query
        name: nextToken
        description: The token for the next set of results, or null if there are no
          additional results
        type: string
      - in: query
        name: thingTypeName
        description: The name of the thing type used to search for things
        type: string
      responses:
        200:
          description: OK
      tags:
      - things
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