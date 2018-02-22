---
swagger: "2.0"
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetComplianceDetailsByResource&k=1:
    get:
      summary: ' Get Compliance Details By Resource '
      description: Returns the evaluation results for the specified AWS resource
      operationId: getComplianceDetailsByResource
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: NextToken
        description: "The nextToken string returned on a previous page that\t\t\tyou
          use to get the next page of results in a paginated response"
        type: string
      - in: query
        name: ResourceId
        description: The ID of the AWS resource for which you want compliance information
        type: string
      - in: query
        name: ResourceType
        description: The type of the AWS resource for which you want compliance information
        type: string
      responses:
        200:
          description: OK
      tags:
      - compliance
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