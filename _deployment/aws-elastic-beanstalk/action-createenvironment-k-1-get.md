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
  /?Action=CreateEnvironment&k=1:
    get:
      summary: ' Create Environment '
      description: |-
        Launches an environment for the specified application using the specified
              configuration
      operationId: createEnvironment
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application that contains the version to be deployed
        type: string
      - in: query
        name: CNAMEPrefix
        description: If specified, the environment attempts to use this value as the
          prefix for the CNAME
        type: string
      - in: query
        name: Description
        description: Describes this environment
        type: string
      - in: query
        name: EnvironmentName
        description: A unique name for the deployment environment
        type: string
      - in: query
        name: GroupName
        description: The name of the group to which the target environment belongs
        type: string
      - in: query
        name: OptionSettings.member.N
        description: If specified, AWS Elastic Beanstalk sets the specified configuration
          options to the      requested value in the configuration set for the new
          environment
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: A list of custom user-defined configuration options to remove
          from the configuration      set for this new environment
        type: string
      - in: query
        name: SolutionStackName
        description: This is an alternative to specifying a template name
        type: string
      - in: query
        name: Tags.member.N
        description: This specifies the tags applied to resources in the environment
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to use in deployment
        type: string
      - in: query
        name: Tier
        description: This specifies the tier to use for creating this environment
        type: string
      - in: query
        name: VersionLabel
        description: The name of the application version to deploy
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