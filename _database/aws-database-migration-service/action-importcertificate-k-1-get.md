---
swagger: "2.0"
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ImportCertificate&k=1:
    get:
      summary: ' Import Certificate '
      description: Uploads the specified certificate
      operationId: importCertificate
      parameters:
      - in: query
        name: CertificateIdentifier
        description: The customer-assigned name of the certificate
        type: string
      - in: query
        name: CertificatePem
        description: 'The contents of the '
        type: string
      - in: query
        name: CertificateWallet
        description: The location of the imported Oracle Wallet certificate for use
          with SSL
        type: string
      responses:
        200:
          description: OK
      tags:
      - certificates
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