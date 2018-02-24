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
  /?Action=CreateThing&k=1:
    get:
      summary: ' Create Thing '
      description: Creates a thing record in the thing registry
      operationId: createThing
      parameters:
      - in: query
        name: attributePayload
        description: The attribute payload, which consists of up to three name/value
          pairs in a JSON document
        type: string
      - in: query
        name: thingName
        description: The name of the thing to create
        type: string
      - in: query
        name: thingTypeName
        description: The name of the thing type associated with the new thing
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