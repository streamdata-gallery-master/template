---
swagger: "2.0"
info:
  title: AWS WorkDocs API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeUsers&k=1:
    get:
      summary: ' Describe Users '
      description: Describes the specified users
      operationId: describeUsers
      parameters:
      - in: query
        name: Fields
        description: A comma-separated list of values
        type: string
      - in: query
        name: Include
        description: The state of the users
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Order
        description: The order for the results
        type: string
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      - in: query
        name: Query
        description: A query to filter users by user name
        type: string
      - in: query
        name: Sort
        description: The sorting criteria
        type: string
      - in: query
        name: UserIds
        description: The IDs of the users
        type: string
      responses:
        200:
          description: OK
      tags:
      - users
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