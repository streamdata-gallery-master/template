---
swagger: "2.0"
info:
  title: AWS Simple Notification Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListSubscriptionsByTopic&k=1:
    get:
      summary: ' List Subscriptions By Topic '
      description: Returns a list of the subscriptions to a specific topic
      operationId: listSubscriptionsByTopic
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListSubscriptionsByTopic request
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic for which you wish to find subscriptions
        type: string
      responses:
        200:
          description: OK
      tags:
      - subscriptions
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