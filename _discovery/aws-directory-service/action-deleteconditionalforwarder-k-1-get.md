---
swagger: "2.0"
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteConditionalForwarder&k=1:
    get:
      summary: ' Delete Conditional Forwarder '
      description: Deletes a conditional forwarder that has been set up for your AWS
        directory
      operationId: deleteConditionalForwarder
      parameters:
      - in: query
        name: DirectoryId
        description: The directory ID for which you are deleting the conditional forwarder
        type: string
      - in: query
        name: RemoteDomainName
        description: The fully qualified domain name (FQDN) of the remote domain with
          which you are deleting the conditional forwarder
        type: string
      responses:
        200:
          description: OK
      tags:
      - conditional forwarder
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