---
swagger: "2.0"
info:
  title: AWs Cognito Identity Provider API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AdminUpdateDeviceStatus&k=1:
    get:
      summary: ' Admin Update Device Status '
      description: Updates the device status as an administrator
      operationId: adminUpdateDeviceStatus
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceRememberedStatus
        description: The status indicating whether a device has been remembered or
          not
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - users
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