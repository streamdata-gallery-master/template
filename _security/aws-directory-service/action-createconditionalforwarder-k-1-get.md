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
  /?Action=CreateConditionalForwarder&k=1:
    get:
      summary: ' Create Conditional Forwarder '
      description: Creates a conditional forwarder associated with your AWS directory
      operationId: createConditionalForwarder
      parameters:
      - in: query
        name: DirectoryId
        description: The directory ID of the AWS directory for which you are creating
          the conditional forwarder
        type: string
      - in: query
        name: DnsIpAddrs
        description: The IP addresses of the remote DNS server associated with RemoteDomainName
        type: string
      - in: query
        name: RemoteDomainName
        description: The fully qualified domain name (FQDN) of the remote domain with
          which you will set up a trust relationship
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