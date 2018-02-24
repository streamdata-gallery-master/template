---
swagger: "2.0"
info:
  title: User Billing History API
  description: The API for managing CloudFlare User Billing History
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
  /user/billing/history:
    get:
      summary: Access your billing history object
      description: Access your billing history object
      operationId: cloudflare-user-billing-history-api
      parameters:
      - in: query
        name: action
        description: The billing item actionsubscription
      - in: query
        name: occured_at
        description: When the billing item was created2014-03-01T12:21:59
      - in: query
        name: order
        description: Field to order billing history byoccured_at
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of items per page20
      - in: query
        name: type
        description: The billing item typecharge
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
      - billing history
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