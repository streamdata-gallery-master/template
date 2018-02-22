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
  /?Action=SetRepositoryPolicy&k=1:
    get:
      summary: ' Set Repository Policy '
      description: Applies a repository policy on a specified repository to control
        access permissions
      operationId: setRepositoryPolicy
      parameters:
      - in: query
        name: force
        description: If the policy you are attempting to set on a repository policy
          would prevent you from            setting another policy in the future,
          you must force the SetRepositoryPolicy            operation
        type: string
      - in: query
        name: policyText
        description: The JSON repository policy text to apply to the repository
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repository
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository to receive the policy
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