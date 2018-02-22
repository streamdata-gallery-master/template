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
  /?Action=UpdateStack&k=1:
    get:
      summary: ' Update Stack '
      description: Updates a stack as specified in the template
      operationId: updateStack
      parameters:
      - in: query
        name: Capabilities.member.N
        description: A list of values that you must specify before AWS CloudFormation
          can update certain stacks
        type: string
      - in: query
        name: NotificationARNs.member.N
        description: Amazon Simple Notification Service topic Amazon Resource Names
          (ARNs) that AWS CloudFormation associates with the stack
        type: string
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
          for the stack
        type: string
      - in: query
        name: ResourceTypes.member.N
        description: The template resource types that you have permissions to work
          with for this update stack action, such as AWS::EC2::Instance, AWS::EC2::*,
          or Custom::MyCustomInstance
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to update
          the stack
        type: string
      - in: query
        name: StackName
        description: The name or unique stack ID of the stack to update
        type: string
      - in: query
        name: StackPolicyBody
        description: Structure containing a new stack policy body
        type: string
      - in: query
        name: StackPolicyDuringUpdateBody
        description: Structure containing the temporary overriding stack policy body
        type: string
      - in: query
        name: StackPolicyDuringUpdateURL
        description: Location of a file containing the temporary overriding stack
          policy
        type: string
      - in: query
        name: StackPolicyURL
        description: Location of a file containing the updated stack policy
        type: string
      - in: query
        name: Tags.member.N
        description: Key-value pairs to associate with this stack
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      - in: query
        name: UsePreviousTemplate
        description: Reuse the existing template that is associated with the stack
          that you are updating
        type: string
      responses:
        200:
          description: OK
      tags:
      - stacks
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