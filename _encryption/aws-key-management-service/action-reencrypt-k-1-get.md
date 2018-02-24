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
  /?Action=ReEncrypt&k=1:
    get:
      summary: ' Re Encrypt '
      description: |-
        Encrypts data on the server side with a new customer master key (CMK) without exposing
              the plaintext of the data on the client side
      operationId: reEncrypt
      parameters:
      - in: query
        name: CiphertextBlob
        description: Ciphertext of the data to reencrypt
        type: string
      - in: query
        name: DestinationEncryptionContext
        description: Encryption context to use when the data is reencrypted
        type: string
      - in: query
        name: DestinationKeyId
        description: A unique identifier for the CMK to use to reencrypt the data
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: SourceEncryptionContext
        description: Encryption context used to encrypt and decrypt the data specified
          in the        CiphertextBlob parameter
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