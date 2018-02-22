---
swagger: "2.0"
info:
  title: AWS ElastiCache API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEvents&k=1:
    get:
      summary: ' Describe Events '
      description: |-
        Returns events related to cache clusters, cache
                    security groups, and cache parameter groups
      operationId: describeEvents
      parameters:
      - in: query
        name: Duration
        description: The number of minutes' worth of events to retrieve
        type: string
      - in: query
        name: EndTime
        description: The end of the time interval for which to retrieve events, specified
          in ISO 8601 format
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SourceIdentifier
        description: The identifier of the event source for which events are returned
        type: string
      - in: query
        name: SourceType
        description: The event source to retrieve events for
        type: string
      - in: query
        name: StartTime
        description: The beginning of the time interval to retrieve events for, specified
          in ISO 8601 format
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
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