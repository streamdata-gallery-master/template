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
  /?Action=ResendValidationEmail&k=1:
    get:
      summary: Resend Validation Email
      description: Resends the email that requests domain ownership validation
      operationId: ResendValidationEmail
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the requested certificate
        type: string
      - in: query
        name: Domain
        description: The Fully Qualified Domain Name (FQDN) of the certificate that
          needs to be      validated
        type: string
      - in: query
        name: ValidationDomain
        description: The base validation domain that will act as the suffix of the
          email addresses that are      used to send the emails
        type: string
      responses:
        200:
          description: OK
      tags:
      - validation email
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