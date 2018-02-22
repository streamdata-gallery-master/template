---
swagger: "2.0"
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeApplicationVersions&k=1:
    get:
      summary: ' Describe Application Versions '
      description: Retrieve a list of application versions
      operationId: describeApplicationVersions
      parameters:
      - in: query
        name: ApplicationName
        description: Specify an application name to show only application versions
          for that      application
        type: string
      - in: query
        name: MaxRecords
        description: Specify a maximum number of application versions to paginate
          in the request
        type: string
      - in: query
        name: NextToken
        description: Specify a next token to retrieve the next page in a paginated
          request
        type: string
      - in: query
        name: VersionLabels.member.N
        description: Specify a version label to show a specific application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - application version
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