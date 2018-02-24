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
  /?Action=CreateStack&k=1:
    get:
      summary: ' Create Stack '
      description: Creates a stack as specified in the template
      operationId: createStack
      parameters:
      - in: query
        name: Capabilities.member.N
        description: A list of values that you must specify before AWS CloudFormation
          can create certain stacks
        type: string
      - in: query
        name: DisableRollback
        description: Set to true to disable rollback of the stack if stack creation
          failed
        type: string
      - in: query
        name: NotificationARNs.member.N
        description: The Simple Notification Service (SNS) topic ARNs to publish stack
          related events
        type: string
      - in: query
        name: OnFailure
        description: Determines what action will be taken if stack creation fails
        type: string
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
          for the stack
        type: string
      - in: query
        name: ResourceTypes.member.N
        description: The template resource types that you have permissions to work
          with for this create stack action, such as AWS::EC2::Instance, AWS::EC2::*,
          or Custom::MyCustomInstance
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to create
          the stack
        type: string
      - in: query
        name: StackName
        description: The name that is associated with the stack
        type: string
      - in: query
        name: StackPolicyBody
        description: Structure containing the stack policy body
        type: string
      - in: query
        name: StackPolicyURL
        description: Location of a file containing the stack policy
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
        name: TimeoutInMinutes
        description: The amount of time that can pass before the stack status becomes
          CREATE_FAILED; if DisableRollback         is not set or is set to false,
          the stack will be rolled back
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