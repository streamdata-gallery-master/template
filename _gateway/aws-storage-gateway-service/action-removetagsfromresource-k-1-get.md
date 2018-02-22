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
  /?Action=RemoveTagsFromResource&k=1:
    get:
      summary: ' Remove Tags From Resource '
      description: Removes one or more tags from the specified resource
      operationId: removeTagsFromResource
      parameters:
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource you want to remove
          the tags         from
        type: string
      - in: query
        name: TagKeys
        description: The keys of the tags you want to remove from the specified resource
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