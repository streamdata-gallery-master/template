---
swagger: "2.0"
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListTagsForResource&k=1:
    get:
      summary: ' List Tags For Resource '
      description: Lists the tags that have been added to the specified resource
      operationId: listTagsForResource
      parameters:
      - in: query
        name: Limit
        description: Specifies that the list of tags returned be limited to the specified
          number of         items
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          returning the list of         tags
        type: string
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource for which you
          want to list         tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - tags
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