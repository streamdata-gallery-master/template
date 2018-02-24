---
swagger: "2.0"
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeConditionalForwarders&k=1:
    get:
      summary: ' Describe Conditional Forwarders '
      description: Obtains information about the conditional forwarders for this account
      operationId: describeConditionalForwarders
      parameters:
      - in: query
        name: DirectoryId
        description: The directory ID for which to get the list of associated conditional
          forwarders
        type: string
      - in: query
        name: RemoteDomainNames
        description: The fully qualified domain names (FQDN) of the remote domains
          for which to get the list of associated conditional forwarders
        type: string
      responses:
        200:
          description: OK
      tags:
      - conditional forwarder
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