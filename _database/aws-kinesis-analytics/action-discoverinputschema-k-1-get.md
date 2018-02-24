---
swagger: "2.0"
info:
  title: AWS Kinesis Analytics API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DiscoverInputSchema&k=1:
    get:
      summary: ' Discover Input Schema '
      description: Infers a schema by evaluating sample records on the specified streaming
        source (Amazon Kinesis stream or Amazon Kinesis Firehose delivery stream)
      operationId: discoverInputSchema
      parameters:
      - in: query
        name: InputStartingPositionConfiguration
        description: Point at which you want Amazon Kinesis Analytics to start reading
          records from the specified streaming source discovery purposes
        type: string
      - in: query
        name: ResourceARN
        description: Amazon Resource Name (ARN) of the streaming source
        type: string
      - in: query
        name: RoleARN
        description: ARN of the IAM role that Amazon Kinesis Analytics can assume
          to access the stream on your behalf
        type: string
      responses:
        200:
          description: OK
      tags:
      - schema
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