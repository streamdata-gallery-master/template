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
  /?Action=EnableLogging&k=1:
    get:
      summary: ' Enable Logging '
      description: |-
        Starts logging information, such as queries and connection attempts, for the
                    specified Amazon Redshift cluster
      operationId: enableLogging
      parameters:
      - in: query
        name: BucketName
        description: The name of an existing S3 bucket where the log files are to
          be stored
        type: string
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster on which logging is to be started
        type: string
      - in: query
        name: S3KeyPrefix
        description: The prefix applied to the log file names
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