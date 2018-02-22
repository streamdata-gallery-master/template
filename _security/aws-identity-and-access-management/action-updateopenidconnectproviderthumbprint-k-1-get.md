---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateOpenIDConnectProviderThumbprint&k=1:
    get:
      summary: ' Update Open I D Connect Provider Thumbprint '
      description: |-
        Replaces the existing list of server certificate thumbprints associated with an OpenID
              Connect (OIDC) provider resource object with a new list of thumbprints
      operationId: updateOpenIDConnectProviderThumbprint
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OIDC provider resource
          object for which you      want to update the thumbprint
        type: string
      - in: query
        name: ThumbprintList.member.N
        description: A list of certificate thumbprints that are associated with the
          specified IAM OpenID      Connect provider
        type: string
      responses:
        200:
          description: OK
      tags:
      - openid connect providers
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