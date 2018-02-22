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
  /?Action=GetParametersForImport&k=1:
    get:
      summary: ' Get Parameters For Import '
      description: |-
        Returns the items you need in order to import key material into AWS KMS from your
              existing key management infrastructure
      operationId: getParametersForImport
      parameters:
      - in: query
        name: KeyId
        description: The identifier of the CMK into which you will import key material
        type: string
      - in: query
        name: WrappingAlgorithm
        description: The algorithm you will use to encrypt the key material before
          importing it with ImportKeyMaterial
        type: string
      - in: query
        name: WrappingKeySpec
        description: The type of wrapping key (public key) to return in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - parameters
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