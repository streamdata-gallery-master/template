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
  /?Action=RequestCertificate&k=1:
    get:
      summary: Request Certificate
      description: Requests an ACM Certificate for use with other AWS services
      operationId: RequestCertificate
      parameters:
      - in: query
        name: DomainName
        description: Fully qualified domain name (FQDN), such as www
        type: string
      - in: query
        name: DomainValidationOptions
        description: The base validation domain that will act as the suffix of the
          email addresses that are      used to send the emails
        type: string
      - in: query
        name: IdempotencyToken
        description: Customer chosen string that can be used to distinguish between
          calls to        RequestCertificate
        type: string
      - in: query
        name: SubjectAlternativeNames
        description: Additional FQDNs to be included in the Subject Alternative Name
          extension of the ACM      Certificate
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