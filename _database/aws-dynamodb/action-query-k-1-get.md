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
  /?Action=Query&k=1:
    get:
      summary: ' Query '
      description: |-
        A Query operation uses the primary key of a table or a secondary index
                    to directly access items from that table or index
      operationId: query
      parameters:
      - in: query
        name: AttributesToGet
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConsistentRead
        description: 'Determines the read consistency model:  If set to true, then
          the operation uses strongly consistent reads; otherwise, the operation uses
          eventually consistent reads'
        type: string
      - in: query
        name: ExclusiveStartKey
        description: The primary key of the first item that this operation will evaluate
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: FilterExpression
        description: A string that contains conditions that DynamoDB applies after
          the Query operation, but       before the data is returned to you
        type: string
      - in: query
        name: IndexName
        description: The name of an index to query
        type: string
      - in: query
        name: KeyConditionExpression
        description: The condition that specifies the key value(s) for items to be
          retrieved by the Query      action
        type: string
      - in: query
        name: KeyConditions
        description: This is a legacy parameter
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to evaluate (not necessarily the
          number of matching items)
        type: string
      - in: query
        name: ProjectionExpression
        description: A string that identifies one or more attributes to retrieve from
          the table
        type: string
      - in: query
        name: QueryFilter
        description: This is a legacy parameter
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ScanIndexForward
        description: 'Specifies the order for index traversal: If true (default),
          the traversal is performed in ascending order; if false, the traversal is
          performed in descending order'
        type: string
      - in: query
        name: Select
        description: The attributes to be returned in the          result
        type: string
      - in: query
        name: TableName
        description: The name of the table containing the requested items
        type: string
      responses:
        200:
          description: OK
      tags:
      - query
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