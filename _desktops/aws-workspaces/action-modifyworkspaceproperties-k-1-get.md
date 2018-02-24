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
  /?Action=ModifyWorkspaceProperties&k=1:
    get:
      summary: ' Modify Workspace Properties '
      description: Modifies the WorkSpace properties, including the running mode and
        AutoStop time
      operationId: modifyWorkspaceProperties
      parameters:
      - in: query
        name: WorkspaceId
        description: The ID of the WorkSpace
        type: string
      - in: query
        name: WorkspaceProperties
        description: The WorkSpace properties of the request
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