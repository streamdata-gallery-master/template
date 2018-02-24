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
  /?Action=CreateEventSubscription&k=1:
    get:
      summary: ' Create Event Subscription '
      description: Creates an Amazon Redshift event notification subscription
      operationId: createEventSubscription
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value; set to true to activate the subscription, set
          to                false to create the subscription but not active it
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: Specifies the Amazon Redshift event categories to be published
          by the event notification            subscription
        type: string
      - in: query
        name: Severity
        description: Specifies the Amazon Redshift event severity to be published
          by the event notification            subscription
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic used to
          transmit the event            notifications
        type: string
      - in: query
        name: SourceIds.SourceId.N
        description: A list of one or more identifiers of Amazon Redshift source objects
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the event subscription to be created
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - event subscriptions
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