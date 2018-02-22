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
  /?Action=DescribeEnvironments&k=1:
    get:
      summary: ' Describe Environments '
      description: Returns descriptions for existing environments
      operationId: describeEnvironments
      parameters:
      - in: query
        name: ApplicationName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that are associated with this application
        type: string
      - in: query
        name: EnvironmentIds.member.N
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that have the specified IDs
        type: string
      - in: query
        name: EnvironmentNames.member.N
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that have the specified names
        type: string
      - in: query
        name: IncludedDeletedBackTo
        description: If specified when IncludeDeleted is set to true, then      environments
          deleted after this date are displayed
        type: string
      - in: query
        name: IncludeDeleted
        description: 'Indicates whether to include deleted environments:'
        type: string
      - in: query
        name: VersionLabel
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that are associated with this application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - environments
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