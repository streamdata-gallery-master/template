---
swagger: "2.0"
info:
  title: AWS Elasticsearch Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2015-01-01/es/domain/{domain_name}/config:
    post:
      summary: ' Update Elasticsearch Domain Config '
      description: |-
        Modifies the configuration of an Amazon ES domain, such as the instance type and the
                        number of instances
      operationId: updateElasticsearchDomainConfig
      responses:
        200:
          description: OK
      tags:
      - domains
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