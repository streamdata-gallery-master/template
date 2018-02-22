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
  /?Action=CreateTable&k=1:
    get:
      summary: ' Create Table '
      description: The CreateTable operation adds a new table to your account
      operationId: createTable
      parameters:
      - in: query
        name: AttributeDefinitions
        description: An array of attributes that describe the key schema for the table
          and indexes
        type: string
      - in: query
        name: GlobalSecondaryIndexes
        description: One or more global secondary indexes (the maximum is five) to
          be created on the table
        type: string
      - in: query
        name: KeySchema
        description: Specifies the attributes that make up the primary key for a table
          or an index
        type: string
      - in: query
        name: LocalSecondaryIndexes
        description: One or more local secondary indexes (the maximum is five) to
          be created on the table
        type: string
      - in: query
        name: ProvisionedThroughput
        description: Represents the provisioned throughput settings for a specified
          table or index
        type: string
      - in: query
        name: StreamSpecification
        description: The settings for DynamoDB Streams on the table
        type: string
      - in: query
        name: TableName
        description: The name of the table to create
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