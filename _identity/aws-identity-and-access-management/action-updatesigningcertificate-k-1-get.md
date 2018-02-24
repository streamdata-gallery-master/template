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
  /?Action=UpdateSigningCertificate&k=1:
    get:
      summary: ' Update Signing Certificate '
      description: |-
        Changes the status of the specified user signing certificate from active to disabled,
              or vice versa
      operationId: updateSigningCertificate
      parameters:
      - in: query
        name: CertificateId
        description: The ID of the signing certificate you want to update
        type: string
      - in: query
        name: Status
        description: The status you want to assign to the certificate
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user the signing certificate belongs to
        type: string
      responses:
        200:
          description: OK
      tags:
      - signing certificates
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