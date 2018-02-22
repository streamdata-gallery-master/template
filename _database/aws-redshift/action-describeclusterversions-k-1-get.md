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
  /?Action=DescribeClusterVersions&k=1:
    get:
      summary: ' Describe Cluster Versions '
      description: Returns descriptions of the available Amazon Redshift cluster versions
      operationId: describeClusterVersions
      parameters:
      - in: query
        name: ClusterParameterGroupFamily
        description: The name of a specific cluster parameter group family to return
          details            for
        type: string
      - in: query
        name: ClusterVersion
        description: The specific cluster version to return
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
      responses:
        200:
          description: OK
      tags:
      - clusters
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