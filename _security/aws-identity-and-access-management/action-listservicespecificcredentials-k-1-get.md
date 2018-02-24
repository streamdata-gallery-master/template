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
  /?Action=ListServiceSpecificCredentials&k=1:
    get:
      summary: ' List Service Specific Credentials '
      description: |-
        Returns information about the service-specific credentials associated with the
              specified IAM user
      operationId: listServiceSpecificCredentials
      parameters:
      - in: query
        name: ServiceName
        description: Filters the returned results to only those for the specified
          AWS service
        type: string
      - in: query
        name: UserName
        description: The name of the user whose service-specific credentials you want
          information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - service specific credentials
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