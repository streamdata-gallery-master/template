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
  /?Action=DescribeTableRestoreStatus&k=1:
    get:
      summary: ' Describe Table Restore Status '
      description: Lists the status of one or more table restore requests made using
        the
      operationId: describeTableRestoreStatus
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The Amazon Redshift cluster that the table is being restored
          to
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous                DescribeTableRestoreStatus
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: TableRestoreRequestId
        description: The identifier of the table restore request to return status
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - tables
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