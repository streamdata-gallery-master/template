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
  /?Action=DeleteTags&k=1:
    get:
      summary: ' Delete Tags '
      description: Deletes a tag or tags from a resource
      operationId: deleteTags
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) from which you want to remove
          the tag or tags
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: The tag key that you want to delete
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