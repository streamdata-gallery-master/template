---
swagger: "2.0"
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateTags&k=1:
    get:
      summary: ' Create Tags '
      description: Adds one or more tags to a specified resource
      operationId: createTags
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) to which you want to add the tag
          or tags
        type: string
      - in: query
        name: Tags.Tag.N
        description: One or more name/value pairs to add as tags to the specified
          resource
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