---
swagger: "2.0"
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutKeyPolicy&k=1:
    get:
      summary: ' Put Key Policy '
      description: Attaches a key policy to the specified customer master key (CMK)
      operationId: putKeyPolicy
      parameters:
      - in: query
        name: BypassPolicyLockoutSafetyCheck
        description: A flag to indicate whether to bypass the key policy lockout safety
          check
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the CMK
        type: string
      - in: query
        name: Policy
        description: The key policy to attach to the CMK
        type: string
      - in: query
        name: PolicyName
        description: The name of the key policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - keys
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