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
  /?Action=CheckIfPhoneNumberIsOptedOut&k=1:
    get:
      summary: ' Check If Phone Number Is Opted Out '
      description: Accepts a phone number and indicates whether the phone holder has
        opted out of receiving SMS messages from your account
      operationId: checkIfPhoneNumberIsOptedOut
      parameters:
      - in: query
        name: phoneNumber
        description: The phone number for which you want to check the opt out status
        type: string
      responses:
        200:
          description: OK
      tags:
      - opt out
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