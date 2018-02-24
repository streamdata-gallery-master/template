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
  /?Action=DeleteTrust&k=1:
    get:
      summary: ' Delete Trust '
      description: Deletes an existing trust relationship between your Microsoft AD
        in the AWS cloud and an external domain
      operationId: deleteTrust
      parameters:
      - in: query
        name: DeleteAssociatedConditionalForwarder
        description: Delete a conditional forwarder as part of a DeleteTrustRequest
        type: string
      - in: query
        name: TrustId
        description: The Trust ID of the trust relationship to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - trust
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