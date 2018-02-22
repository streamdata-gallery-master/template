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
  /?Action=UpdateSnapshotSchedule&k=1:
    get:
      summary: ' Update Snapshot Schedule '
      description: Updates a snapshot schedule configured for a gateway volume
      operationId: updateSnapshotSchedule
      parameters:
      - in: query
        name: Description
        description: Optional description of the snapshot that overwrites the existing         description
        type: string
      - in: query
        name: RecurrenceInHours
        description: Frequency of snapshots
        type: string
      - in: query
        name: StartAt
        description: The hour of the day at which the snapshot schedule begins represented
          as            hh, where hh is the hour (0 to 23)
        type: string
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - snapshots
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