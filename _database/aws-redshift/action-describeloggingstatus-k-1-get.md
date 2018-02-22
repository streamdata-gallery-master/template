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
  /?Action=DescribeLoggingStatus&k=1:
    get:
      summary: ' Describe Logging Status '
      description: |-
        Describes whether information, such as queries and connection attempts, is being
                    logged for the specified Amazon Redshift cluster
      operationId: describeLoggingStatus
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster from which to get the logging status
        type: string
      responses:
        200:
          description: OK
      tags:
      - logging
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