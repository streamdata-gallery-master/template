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
  /?Action=ListCertificates&k=1:
    get:
      summary: List Certificates
      description: Retrieves a list of ACM Certificates and the domain name for each
      operationId: ListCertificates
      parameters:
      - in: query
        name: CertificateStatuses
        description: The status or statuses on which to filter the list of ACM Certificates
        type: string
      - in: query
        name: MaxItems
        description: Use this parameter when paginating results to specify the maximum
          number of items to      return in the response
        type: string
      - in: query
        name: NextToken
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
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