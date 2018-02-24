---
swagger: "2.0"
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutDeliveryChannel&k=1:
    get:
      summary: ' Put Delivery Channel '
      description: Creates a delivery channel object to deliver configuration information
        to an Amazon S3 bucket and Amazon SNS topic
      operationId: putDeliveryChannel
      parameters:
      - in: query
        name: DeliveryChannel
        description: The configuration delivery channel object that delivers the configuration
          information to an Amazon S3 bucket, and to an Amazon SNS topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - delivery channels
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