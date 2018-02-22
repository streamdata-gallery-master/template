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
  /?Action=GetSAMLProvider&k=1:
    get:
      summary: ' Get S A M L Provider '
      description: |-
        Returns the SAML provider metadocument that was uploaded when the IAM SAML provider
              resource object was created or updated
      operationId: getSAMLProvider
      parameters:
      - in: query
        name: SAMLProviderArn
        description: The Amazon Resource Name (ARN) of the SAML provider resource
          object in IAM to get      information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - saml providers
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