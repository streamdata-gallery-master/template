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
  /?Action=DescribeEvents&k=1:
    get:
      summary: ' Describe Events '
      description: Returns list of event descriptions matching criteria up to the
        last 6 weeks
      operationId: describeEvents
      parameters:
      - in: query
        name: ApplicationName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those associated with this application
        type: string
      - in: query
        name: EndTime
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      occur up to, but not including, the EndTime
        type: string
      - in: query
        name: EnvironmentId
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this environment
        type: string
      - in: query
        name: EnvironmentName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this environment
        type: string
      - in: query
        name: MaxRecords
        description: Specifies the maximum number of events that can be returned,
          beginning with the most      recent event
        type: string
      - in: query
        name: NextToken
        description: Pagination token
        type: string
      - in: query
        name: RequestId
        description: If specified, AWS Elastic Beanstalk restricts the described events
          to include only      those associated with this request ID
        type: string
      - in: query
        name: Severity
        description: If specified, limits the events returned from this call to include
          only those with the      specified severity or higher
        type: string
      - in: query
        name: StartTime
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      occur on or after this time
        type: string
      - in: query
        name: TemplateName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      are associated with this environment configuration
        type: string
      - in: query
        name: VersionLabel
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
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