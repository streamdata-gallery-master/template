---
swagger: "2.0"
info:
  title: Users Organizations API
  description: The API for managing CloudFlare User&amp;#x27;s Organizations
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
  /user/organizations:
    get:
      summary: List organizations the user is associated with
      description: List organizations the user is associated with
      operationId: cloudflare-userx27s-organizations-api
      parameters:
      - in: query
        name: direction
        description: Direction to order organizationsdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)all
      - in: query
        name: name
        description: Organization NameCloudFlare, Inc
      - in: query
        name: order
        description: Field to order organizations bystatus
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of organizations per page20
      - in: query
        name: status
        description: Whether or not the user is a member of the organization or has
          an inivitation pendingmember
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
      - user organizations
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