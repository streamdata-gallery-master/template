---
swagger: "2.0"
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ScheduleKeyDeletion&k=1:
    get:
      summary: ' Schedule Key Deletion '
      description: Schedules the deletion of a customer master key (CMK)
      operationId: scheduleKeyDeletion
      parameters:
      - in: query
        name: KeyId
        description: The unique identifier for the customer master key (CMK) to delete
        type: string
      - in: query
        name: PendingWindowInDays
        description: The waiting period, specified in number of days
        type: string
      responses:
        200:
          description: OK
      tags:
      - keys
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