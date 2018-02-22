---
swagger: "2.0"
info:
  title: AWs Cognito Identity Provider API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateUserPool&k=1:
    get:
      summary: ' Update User Pool '
      description: Updates the specified user pool with the specified attributes
      operationId: updateUserPool
      parameters:
      - in: query
        name: AdminCreateUserConfig
        description: The configuration for AdminCreateUser requests
        type: string
      - in: query
        name: AutoVerifiedAttributes
        description: The attributes that are automatically verified when the Amazon
          Cognito service            makes a request to update user pools
        type: string
      - in: query
        name: DeviceConfiguration
        description: Device configuration
        type: string
      - in: query
        name: EmailConfiguration
        description: Email configuration
        type: string
      - in: query
        name: EmailVerificationMessage
        description: The contents of the email verification message
        type: string
      - in: query
        name: EmailVerificationSubject
        description: The subject of the email verification message
        type: string
      - in: query
        name: LambdaConfig
        description: The AWS Lambda configuration information from the request to
          update the user            pool
        type: string
      - in: query
        name: MfaConfiguration
        description: 'Can be one of the following values:'
        type: string
      - in: query
        name: Policies
        description: A container with the policies you wish to update in a user pool
        type: string
      - in: query
        name: SmsAuthenticationMessage
        description: The contents of the SMS authentication message
        type: string
      - in: query
        name: SmsConfiguration
        description: SMS configuration
        type: string
      - in: query
        name: SmsVerificationMessage
        description: A container with information about the SMS verification message
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to update
        type: string
      - in: query
        name: UserPoolTags
        description: The cost allocation tags for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - user pools
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