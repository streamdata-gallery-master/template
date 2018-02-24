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
  /?Action=Encrypt&k=1:
    get:
      summary: ' Encrypt '
      description: Encrypts plaintext into ciphertext by using a customer master key
      operationId: encrypt
      parameters:
      - in: query
        name: EncryptionContext
        description: Name-value pair that specifies the encryption context to be used
          for authenticated      encryption
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      - in: query
        name: Plaintext
        description: Data to be encrypted
        type: string
      responses:
        200:
          description: OK
      tags:
      - encrypt
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