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
  /?Action=DescribeInstancesHealth&k=1:
    get:
      summary: ' Describe Instances Health '
      description: |-
        Retrives detailed information about the health of instances in your AWS Elastic
              Beanstalk
      operationId: describeInstancesHealth
      parameters:
      - in: query
        name: AttributeNames.member.N
        description: Specifies the response elements you wish to receive
        type: string
      - in: query
        name: EnvironmentId
        description: Specify the AWS Elastic Beanstalk environment by ID
        type: string
      - in: query
        name: EnvironmentName
        description: Specify the AWS Elastic Beanstalk environment by name
        type: string
      - in: query
        name: NextToken
        description: Specify the pagination token returned by a previous call
        type: string
      responses:
        200:
          description: OK
      tags:
      - instances health
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