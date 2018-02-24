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
  /?Action=DeletePlatformApplication&k=1:
    get:
      summary: ' Delete Platform Application '
      description: |-
        Deletes a platform application object for one of the supported push notification services,
              such as APNS and GCM
      operationId: deletePlatformApplication
      parameters:
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn of platform application object to delete
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