---
swagger: "2.0"
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdatePortfolio&k=1:
    get:
      summary: ' Update Portfolio '
      description: Updates the specified portfolio's details
      operationId: updatePortfolio
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AddTags
        description: Tags to add to the existing list of tags associated with the
          portfolio
        type: string
      - in: query
        name: Description
        description: The updated text description of the portfolio
        type: string
      - in: query
        name: DisplayName
        description: The name to use for display purposes
        type: string
      - in: query
        name: Id
        description: The identifier of the portfolio for the update request
        type: string
      - in: query
        name: ProviderName
        description: The updated name of the portfolio provider
        type: string
      - in: query
        name: RemoveTags
        description: Tags to remove from the existing list of tags associated with
          the         portfolio
        type: string
      responses:
        200:
          description: OK
      tags:
      - portfolios
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