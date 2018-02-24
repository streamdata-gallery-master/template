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
  /?Action=ImportKeyMaterial&k=1:
    get:
      summary: ' Import Key Material '
      description: |-
        Imports key material into an AWS KMS customer master key (CMK) from your existing key
              management infrastructure
      operationId: importKeyMaterial
      parameters:
      - in: query
        name: EncryptedKeyMaterial
        description: The encrypted key material to import
        type: string
      - in: query
        name: ExpirationModel
        description: Specifies whether the key material expires
        type: string
      - in: query
        name: ImportToken
        description: The import token that you received in the response to a previous
          GetParametersForImport request
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK to import the key material into
        type: string
      - in: query
        name: ValidTo
        description: The time at which the imported key material expires
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