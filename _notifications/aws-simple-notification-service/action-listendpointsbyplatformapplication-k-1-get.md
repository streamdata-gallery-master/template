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
  /?Action=ListEndpointsByPlatformApplication&k=1:
    get:
      summary: ' List Endpoints By Platform Application '
      description: |-
        Lists the endpoints and endpoint attributes for devices in a supported push notification
              service, such as GCM and APNS
      operationId: listEndpointsByPlatformApplication
      parameters:
      - in: query
        name: NextToken
        description: NextToken string is used when calling ListEndpointsByPlatformApplication
          action to retrieve additional records that are available after the first
          page results
        type: string
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn for ListEndpointsByPlatformApplicationInput
          action
        type: string
      responses:
        200:
          description: OK
      tags:
      - endpoints
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