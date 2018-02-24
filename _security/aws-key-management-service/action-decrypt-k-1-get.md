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
  /?Action=Decrypt&k=1:
    get:
      summary: ' Decrypt '
      description: Decrypts ciphertext
      operationId: decrypt
      parameters:
      - in: query
        name: CiphertextBlob
        description: Ciphertext to be decrypted
        type: string
      - in: query
        name: EncryptionContext
        description: The encryption context
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - decrypt
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