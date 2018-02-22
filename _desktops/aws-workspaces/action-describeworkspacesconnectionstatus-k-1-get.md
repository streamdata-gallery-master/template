---
swagger: "2.0"
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeWorkspacesConnectionStatus&k=1:
    get:
      summary: ' Describe Workspaces Connection Status '
      description: Describes the connection status of a specified WorkSpace
      operationId: describeWorkspacesConnectionStatus
      parameters:
      - in: query
        name: NextToken
        description: The next token of the request
        type: string
      - in: query
        name: WorkspaceIds
        description: An array of strings that contain the identifiers of the WorkSpaces
        type: string
      responses:
        200:
          description: OK
      tags:
      - workspaces
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