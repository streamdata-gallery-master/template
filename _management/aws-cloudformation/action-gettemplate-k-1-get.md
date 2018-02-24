---
swagger: "2.0"
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetTemplate&k=1:
    get:
      summary: ' Get Template '
      description: Returns the template body for a specified stack
      operationId: getTemplate
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of a change set for which
          AWS CloudFormation returns the associated template
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      - in: query
        name: TemplateStage
        description: For templates that include transforms, the stage of the template
          that AWS CloudFormation returns
        type: string
      responses:
        200:
          description: OK
      tags:
      - templates
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