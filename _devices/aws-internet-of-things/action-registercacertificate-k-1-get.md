---
swagger: "2.0"
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterCACertificate&k=1:
    get:
      summary: ' Register C A Certificate '
      description: Registers a CA certificate with AWS IoT
      operationId: registerCACertificate
      parameters:
      - in: query
        name: allowAutoRegistration
        description: Allows this CA certificate to be used for auto registration of
          device certificates
        type: string
      - in: query
        name: caCertificate
        description: The CA certificate
        type: string
      - in: query
        name: setAsActive
        description: A boolean value that specifies if the CA certificate is set to
          active
        type: string
      - in: query
        name: verificationCertificate
        description: The private key verification certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - ca certificates
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