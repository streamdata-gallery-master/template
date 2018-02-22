---
swagger: "2.0"
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTagsToResource&k=1:
    get:
      summary: ' Add Tags To Resource '
      description: Adds or overwrites one or more tags for the specified directory
      operationId: addTagsToResource
      parameters:
      - in: query
        name: ResourceId
        description: Identifier (ID) for the directory to which to add the tag
        type: string
      - in: query
        name: Tags
        description: The tags to be assigned to the directory
        type: string
      responses:
        200:
          description: OK
      tags:
      - resource tags
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