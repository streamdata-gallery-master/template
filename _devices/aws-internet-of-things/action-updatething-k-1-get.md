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
  /?Action=UpdateThing&k=1:
    get:
      summary: ' Update Thing '
      description: Updates the data for a thing
      operationId: updateThing
      parameters:
      - in: query
        name: attributePayload
        description: A list of thing attributes, a JSON string containing name-value
          pairs
        type: string
      - in: query
        name: expectedVersion
        description: The expected version of the thing record in the registry
        type: string
      - in: query
        name: removeThingType
        description: Remove a thing type association
        type: string
      - in: query
        name: thingName
        description: The name of the thing to update
        type: string
      - in: query
        name: thingTypeName
        description: The name of the thing type
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