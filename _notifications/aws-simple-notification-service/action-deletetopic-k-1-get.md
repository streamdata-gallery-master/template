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
  /?Action=DeleteTopic&k=1:
    get:
      summary: ' Delete Topic '
      description: Deletes a topic and all its subscriptions
      operationId: deleteTopic
      parameters:
      - in: query
        name: TopicArn
        description: The ARN of the topic you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - topics
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