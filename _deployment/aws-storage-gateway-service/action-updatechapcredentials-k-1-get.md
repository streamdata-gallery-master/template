---
swagger: "2.0"
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateChapCredentials&k=1:
    get:
      summary: ' Update Chap Credentials '
      description: |-
        Updates the Challenge-Handshake Authentication Protocol (CHAP) credentials for a
                 specified iSCSI target
      operationId: updateChapCredentials
      parameters:
      - in: query
        name: InitiatorName
        description: The iSCSI initiator that connects to the target
        type: string
      - in: query
        name: SecretToAuthenticateInitiator
        description: The secret key that the initiator (for example, the Windows client)
          must provide to         participate in mutual CHAP with the target
        type: string
      - in: query
        name: SecretToAuthenticateTarget
        description: The secret key that the target must provide to participate in
          mutual CHAP with the         initiator (e
        type: string
      - in: query
        name: TargetARN
        description: The Amazon Resource Name (ARN) of the iSCSI volume target
        type: string
      responses:
        200:
          description: OK
      tags:
      - chap credentials
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