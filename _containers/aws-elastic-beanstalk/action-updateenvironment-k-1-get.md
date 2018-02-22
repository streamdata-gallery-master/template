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
  /?Action=UpdateEnvironment&k=1:
    get:
      summary: ' Update Environment '
      description: |-
        Updates the environment description, deploys a new application version, updates the
              configuration settings to an entirely new configuration template, or updates select
              configuration option values in the running environment
      operationId: updateEnvironment
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application with which the environment is associated
        type: string
      - in: query
        name: Description
        description: If this parameter is specified, AWS Elastic Beanstalk updates
          the description of this      environment
        type: string
      - in: query
        name: EnvironmentId
        description: The ID of the environment to update
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to update
        type: string
      - in: query
        name: GroupName
        description: The name of the group to which the target environment belongs
        type: string
      - in: query
        name: OptionSettings.member.N
        description: If specified, AWS Elastic Beanstalk updates the configuration
          set associated with the      running environment and sets the specified
          configuration options to the requested      value
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: A list of custom user-defined configuration options to remove
          from the configuration      set for this environment
        type: string
      - in: query
        name: SolutionStackName
        description: This specifies the platform version that the environment will
          run after the environment      is updated
        type: string
      - in: query
        name: TemplateName
        description: If this parameter is specified, AWS Elastic Beanstalk deploys
          this configuration      template to the environment
        type: string
      - in: query
        name: Tier
        description: This specifies the tier to use to update the environment
        type: string
      - in: query
        name: VersionLabel
        description: If this parameter is specified, AWS Elastic Beanstalk deploys
          the named application      version to the environment
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