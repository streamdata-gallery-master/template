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
  /?Action=DescribeTrusts&k=1:
    get:
      summary: ' Describe Trusts '
      description: Obtains information about the trust relationships for this account
      operationId: describeTrusts
      parameters:
      - in: query
        name: DirectoryId
        description: The Directory ID of the AWS directory that is a part of the requested
          trust relationship
        type: string
      - in: query
        name: Limit
        description: The maximum number of objects to return
        type: string
      - in: query
        name: NextToken
        description: The DescribeTrustsResult
        type: string
      - in: query
        name: TrustIds
        description: A list of identifiers of the trust relationships for which to
          obtain the information
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