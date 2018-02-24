---
swagger: "2.0"
info:
  title: Google Cloud Pub/Sub
  description: Provides reliable, many-to-many, asynchronous messaging between applications.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: pubsub.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{subscription}:modifyAckDeadline:
    post:
      summary: Modify ACK Deadline
      description: Modifies the ack deadline for a specific message
      operationId: pubsub.projects.subscriptions.modifyAckDeadline
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription
        description: The name of the subscription
      responses:
        200:
          description: OK
      tags:
      - ack deadline
definitions:
  AcknowledgeRequest:
    properties:
      ackIds:
        description: This is a default description.
        type: post
  Binding:
    properties:
      members:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
  Empty:
    properties: []
  ListSubscriptionsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      subscriptions:
        description: This is a default description.
        type: post
  ListTopicSubscriptionsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      subscriptions:
        description: This is a default description.
        type: post
  ListTopicsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      topics:
        description: This is a default description.
        type: post
  ModifyAckDeadlineRequest:
    properties:
      ackDeadlineSeconds:
        description: This is a default description.
        type: post
      ackIds:
        description: This is a default description.
        type: post
  ModifyPushConfigRequest:
    properties: []
  Policy:
    properties:
      bindings:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  PublishRequest:
    properties:
      messages:
        description: This is a default description.
        type: post
  PublishResponse:
    properties:
      messageIds:
        description: This is a default description.
        type: post
  PubsubMessage:
    properties:
      attributes:
        description: This is a default description.
        type: post
      data:
        description: This is a default description.
        type: post
      messageId:
        description: This is a default description.
        type: post
      publishTime:
        description: This is a default description.
        type: post
  PullRequest:
    properties:
      maxMessages:
        description: This is a default description.
        type: post
      returnImmediately:
        description: This is a default description.
        type: post
  PullResponse:
    properties:
      receivedMessages:
        description: This is a default description.
        type: post
  PushConfig:
    properties:
      attributes:
        description: This is a default description.
        type: post
      pushEndpoint:
        description: This is a default description.
        type: post
  ReceivedMessage:
    properties:
      ackId:
        description: This is a default description.
        type: post
  SetIamPolicyRequest:
    properties: []
  Subscription:
    properties:
      ackDeadlineSeconds:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      topic:
        description: This is a default description.
        type: post
  TestIamPermissionsRequest:
    properties:
      permissions:
        description: This is a default description.
        type: post
  TestIamPermissionsResponse:
    properties:
      permissions:
        description: This is a default description.
        type: post
  Topic:
    properties:
      name:
        description: This is a default description.
        type: post
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