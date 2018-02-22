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
  /?Action=DeleteRepositoryPolicy&k=1:
    get:
      summary: ' Delete Repository Policy '
      description: Deletes the repository policy from a specified repository
      operationId: deleteRepositoryPolicy
      parameters:
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repository policy to delete
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository that is associated with the repository
          policy to delete
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