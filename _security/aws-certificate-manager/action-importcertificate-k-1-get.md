---
swagger: "2.0"
info:
  title: AWS Certificate Manager API
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
      summary: Import Certificate
      description: Imports an SSL/TLS certificate into AWS Certificate Manager (ACM)
        to use with
      operationId: ImportCertificate
      parameters:
      - in: query
        name: Certificate
        description: The certificate to import
        type: string
      - in: query
        name: CertificateArn
        description: The Amazon Resource Name        (ARN) of an imported certificate
          to replace
        type: string
      - in: query
        name: CertificateChain
        description: The certificate chain
        type: string
      - in: query
        name: PrivateKey
        description: The private key that matches the public key in the certificate
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