---
swagger: "2.0"
info:
  title: AWS EC2 Container Registry API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetRepositoryPolicy&k=1:
    get:
      summary: ' Get Repository Policy '
      description: Retrieves the repository policy for a specified repository
      operationId: getRepositoryPolicy
      parameters:
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repository
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository whose policy you want to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - repository policies
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