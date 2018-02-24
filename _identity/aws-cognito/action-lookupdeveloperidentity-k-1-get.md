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
  /?Action=LookupDeveloperIdentity&k=1:
    get:
      summary: ' Lookup Developer Identity '
      description: |-
        Retrieves the IdentityID associated with a
                    DeveloperUserIdentifier or the list of
                 DeveloperUserIdentifiers associated with an IdentityId for an
                 existing identity
      operationId: lookupDeveloperIdentity
      parameters:
      - in: query
        name: DeveloperUserIdentifier
        description: A unique ID used by your backend authentication process to identify
          a user
        type: string
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of identities to return
        type: string
      - in: query
        name: NextToken
        description: A pagination token
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