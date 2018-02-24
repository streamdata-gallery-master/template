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
  /?Action=Publish&k=1:
    get:
      summary: ' Publish '
      description: Sends a message to all of a topic's subscribed endpoints
      operationId: publish
      parameters:
      - in: query
        name: Message
        description: The message you want to send to the topic
        type: string
      - in: query
        name: |-
          MessageAttributes
                      , MessageAttributes.entry.N.Name (key), MessageAttributesentry.N.Value (value)
        description: Message attributes for Publish action
        type: string
      - in: query
        name: MessageStructure
        description: Set MessageStructure to json if you want to send a different      message
          for each protocol
        type: string
      - in: query
        name: PhoneNumber
        description: The phone number to which you want to deliver an SMS message
        type: string
      - in: query
        name: Subject
        description: Optional parameter to be used as the Subject line when the message
          is delivered to email endpoints
        type: string
      - in: query
        name: TargetArn
        description: Either TopicArn or EndpointArn, but not both
        type: string
      - in: query
        name: TopicArn
        description: The topic you want to publish to
        type: string
      responses:
        200:
          description: OK
      tags:
      - publish
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