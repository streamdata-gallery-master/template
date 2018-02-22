---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateGroup&k=1:
    get:
      summary: ' Update Group '
      description: Updates the name and/or the path of the specified IAM group
      operationId: updateGroup
      parameters:
      - in: query
        name: GroupName
        description: Name of the IAM group to update
        type: string
      - in: query
        name: NewGroupName
        description: New name for the IAM group
        type: string
      - in: query
        name: NewPath
        description: New path for the IAM group
        type: string
      responses:
        200:
          description: OK
      tags:
      - groups
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