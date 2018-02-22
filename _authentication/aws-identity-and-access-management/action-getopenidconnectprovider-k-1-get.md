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
  /?Action=GetOpenIDConnectProvider&k=1:
    get:
      summary: ' Get Open I D Connect Provider '
      description: |-
        Returns information about the specified OpenID Connect (OIDC) provider resource object
              in IAM
      operationId: getOpenIDConnectProvider
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the OIDC provider resource
          object in IAM to get      information for
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