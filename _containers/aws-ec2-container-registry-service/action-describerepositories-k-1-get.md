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
  /?Action=DescribeRepositories&k=1:
    get:
      summary: ' Describe Repositories '
      description: Describes image repositories in a registry
      operationId: describeRepositories
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of repository results returned by DescribeRepositories
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                DescribeRepositories
          request where maxResults was used and            the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repositories to be described
        type: string
      - in: query
        name: repositoryNames
        description: A list of repositories to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - repositories
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