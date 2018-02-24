---
swagger: "2.0"
info:
  title: AWS DynamoDB API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeLimits&k=1:
    get:
      summary: ' Describe Limits '
      description: Returns the current provisioned-capacity limits for your AWS account
        in a region, both for the region as a whole and for any one DynamoDB table
        that you create there
      operationId: describeLimits
      parameters:
      - in: query
        name: AccountMaxReadCapacityUnits
        description: The maximum total read capacity units that your account allows
          you to provision across all of your tables in this region
        type: string
      - in: query
        name: AccountMaxWriteCapacityUnits
        description: The maximum total write capacity units that your account allows
          you to provision across all of your tables in this region
        type: string
      - in: query
        name: TableMaxReadCapacityUnits
        description: The maximum read capacity units that your account allows you
          to provision for a new table that you are creating in this region, including
          the read capacity units provisioned for its global secondary indexes (GSIs)
        type: string
      - in: query
        name: TableMaxWriteCapacityUnits
        description: The maximum write capacity units that your account allows you
          to provision for a new table that you are creating in this region, including
          the write capacity units provisioned for its global secondary indexes (GSIs)
        type: string
      responses:
        200:
          description: OK
      tags:
      - limits
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