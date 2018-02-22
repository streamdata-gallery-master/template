---
swagger: "2.0"
info:
  title: Google OAuth2
  description: Obtains end-user authorization grants for use with other Google APIs.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth2/v2/certs:
    get:
      summary: Get Certificate
      description: Get the certification for this session
      operationId: oauth2.getCertForOpenIdConnect
      responses:
        200:
          description: OK
      tags:
      - certificate
definitions:
  Jwk:
    properties:
      keys:
        description: This is a default description.
        type: parameters
  Tokeninfo:
    properties:
      access_type:
        description: This is a default description.
        type: parameters
      audience:
        description: This is a default description.
        type: parameters
      email:
        description: This is a default description.
        type: parameters
      expires_in:
        description: This is a default description.
        type: parameters
      issued_to:
        description: This is a default description.
        type: parameters
      scope:
        description: This is a default description.
        type: parameters
      token_handle:
        description: This is a default description.
        type: parameters
      user_id:
        description: This is a default description.
        type: parameters
      verified_email:
        description: This is a default description.
        type: parameters
  Userinfoplus:
    properties:
      email:
        description: This is a default description.
        type: parameters
      family_name:
        description: This is a default description.
        type: parameters
      gender:
        description: This is a default description.
        type: parameters
      given_name:
        description: This is a default description.
        type: parameters
      hd:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      link:
        description: This is a default description.
        type: parameters
      locale:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      picture:
        description: This is a default description.
        type: parameters
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