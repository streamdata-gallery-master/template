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
  /?Action=DescribeTags&k=1:
    get:
      summary: ' Describe Tags '
      description: Returns a list of tags
      operationId: describeTags
      parameters:
      - in: query
        name: Marker
        description: A value that indicates the starting point for the next set of
          response records in a            subsequent request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number or response records to return in each call
        type: string
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) for which you want to describe
          the tag or tags
        type: string
      - in: query
        name: ResourceType
        description: The type of resource with which you want to view tags
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching resources
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          resources that are            associated with the specified value or values
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