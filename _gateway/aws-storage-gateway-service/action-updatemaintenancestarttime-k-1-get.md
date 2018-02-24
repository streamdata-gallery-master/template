---
swagger: "2.0"
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateMaintenanceStartTime&k=1:
    get:
      summary: ' Update Maintenance Start Time '
      description: |-
        Updates a gateway's weekly maintenance start time information, including day and time
                 of the week
      operationId: updateMaintenanceStartTime
      parameters:
      - in: query
        name: DayOfWeek
        description: The maintenance start time day of the week represented as an
          ordinal number from 0 to 6,          where 0 represents Sunday and 6 Saturday
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: HourOfDay
        description: The hour component of the maintenance start time represented
          as            hh, where hh is the hour (00 to 23)
        type: string
      - in: query
        name: MinuteOfHour
        description: The minute component of the maintenance start time represented
          as            mm, where mm is the minute (00 to 59)
        type: string
      responses:
        200:
          description: OK
      tags:
      - maintenance
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