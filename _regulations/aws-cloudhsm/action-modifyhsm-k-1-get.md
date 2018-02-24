---
swagger: "2.0"
info:
  title: AWS CloudHSM API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyHsm&k=1:
    get:
      summary: ' Modify HSM '
      description: Modifies an HSM
      operationId: modifyHsm
      parameters:
      - in: query
        name: EniIp
        description: The new IP address for the elastic network interface (ENI) attached
          to the      HSM
        type: string
      - in: query
        name: ExternalId
        description: The new external ID
        type: string
      - in: query
        name: HsmArn
        description: The ARN of the HSM to modify
        type: string
      - in: query
        name: IamRoleArn
        description: The new IAM role ARN
        type: string
      - in: query
        name: SubnetId
        description: The new identifier of the subnet that the HSM is in
        type: string
      - in: query
        name: SyslogIp
        description: The new IP address for the syslog monitoring server
        type: string
      responses:
        200:
          description: OK
      tags:
      - hsm instances
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