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
  /?Action=DescribeConfigurationOptions&k=1:
    get:
      summary: ' Describe Configuration Options '
      description: |-
        Describes the configuration options that are used in a particular configuration
              template or environment, or that a specified solution stack defines
      operationId: describeConfigurationOptions
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application associated with the configuration
          template or environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment whose configuration options you want
          to describe
        type: string
      - in: query
        name: Options.member.N
        description: If specified, restricts the descriptions to only the specified
          options
        type: string
      - in: query
        name: SolutionStackName
        description: The name of the solution stack whose configuration options you
          want to      describe
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template whose configuration options
          you want to      describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - configurationoptions
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