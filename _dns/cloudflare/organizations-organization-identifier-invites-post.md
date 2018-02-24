---
swagger: "2.0"
info:
  title: Organization Invites API
  description: The API for managing CloudFlare Organization Invites
  termsOfService: https://www.cloudflare.com/terms/
  version: 1.0.0
host: api.cloudflare.com
basePath: /client/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/:organization_identifier/invites:
    post:
      summary: Invite a User to become a Member of an Organization
      description: Invite a User to become a Member of an Organization
      operationId: cloudflare-organization-invites-api
      parameters:
      - in: query
        name: invited_member_email
        description: Email address of the user to be added to the Organizationttttttttttttttuser@example
      - in: query
        name: roles
        description: Array of Roles associated with the invited usertttttttttttttt[{id:5a7805061c76ada191ed06f989cc3dac},{id:9a7806061c88ada191ed06f989cc3dac}]
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - organization invites
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