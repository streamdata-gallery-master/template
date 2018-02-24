---
swagger: "2.0"
info:
  title: AWS Cognito API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=MergeDeveloperIdentities&k=1:
    get:
      summary: ' Merge Developer Identities '
      description: |-
        Merges two users having different IdentityIds, existing in the same
                 identity pool, and identified by the same developer provider
      operationId: mergeDeveloperIdentities
      parameters:
      - in: query
        name: DestinationUserIdentifier
        description: User identifier for the destination user
        type: string
      - in: query
        name: DeveloperProviderName
        description: The domain by which Cognito will refer to your users
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: SourceUserIdentifier
        description: User identifier for the source user
        type: string
      responses:
        200:
          description: OK
      tags:
      - developer identities
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