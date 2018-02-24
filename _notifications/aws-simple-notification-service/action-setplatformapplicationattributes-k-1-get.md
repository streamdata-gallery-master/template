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
  /?Action=SetPlatformApplicationAttributes&k=1:
    get:
      summary: ' Set Platform Application Attributes '
      description: |-
        Sets the attributes of the platform application object for the supported push notification
              services, such as APNS and GCM
      operationId: setPlatformApplicationAttributes
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: A map of the platform application attributes
        type: string
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn for SetPlatformApplicationAttributes action
        type: string
      responses:
        200:
          description: OK
      tags:
      - platform applications
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