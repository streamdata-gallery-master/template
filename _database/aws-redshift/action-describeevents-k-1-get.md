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
  /?Action=DescribeEvents&k=1:
    get:
      summary: ' Describe Events '
      description: |-
        Returns events related to clusters, security groups, snapshots, and parameter
                    groups for the past 14 days
      operationId: describeEvents
      parameters:
      - in: query
        name: Duration
        description: The number of minutes prior to the time of the request for which
          to retrieve            events
        type: string
      - in: query
        name: EndTime
        description: The end of the time interval for which to retrieve events, specified
          in ISO 8601            format
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SourceIdentifier
        description: The identifier of the event source for which events will be returned
        type: string
      - in: query
        name: SourceType
        description: The event source to retrieve events for
        type: string
      - in: query
        name: StartTime
        description: The beginning of the time interval to retrieve events for, specified
          in ISO 8601            format
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