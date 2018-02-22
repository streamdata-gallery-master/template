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
  /?Action=ConfirmDevice&k=1:
    get:
      summary: ' Confirm Device '
      description: Confirms tracking of the device
      operationId: confirmDevice
      parameters:
      - in: query
        name: AccessToken
        description: The access token
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceName
        description: The device name
        type: string
      - in: query
        name: DeviceSecretVerifierConfig
        description: The configuration of the device secret verifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - devices
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