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
  /?Action=ConfirmSubscription&k=1:
    get:
      summary: ' Confirm Subscription '
      description: |-
        Verifies an endpoint owner's intent to receive messages by validating the token sent to the
              endpoint by an earlier Subscribe action
      operationId: confirmSubscription
      parameters:
      - in: query
        name: AuthenticateOnUnsubscribe
        description: Disallows unauthenticated unsubscribes of the subscription
        type: string
      - in: query
        name: Token
        description: Short-lived token sent to an endpoint during the Subscribe action
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic for which you wish to confirm a subscription
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