---
swagger: "2.0"
info:
  title: Google Cloud Speech
  description: Google Cloud Speech API.
  contact:
    name: Google
    url: https://google.com
  version: v1beta1
host: speech.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1beta1/speech:asyncrecognize:
    post:
      summary: Perform Asynchronous Speech Recognition
      description: |-
        Performs asynchronous speech recognition: receive results via the
        [google
      operationId: speech.speech.asyncrecognize
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - speech recognition
definitions:
  AsyncRecognizeRequest:
    properties: []
  Empty:
    properties: []
  ListOperationsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      operations:
        description: This is a default description.
        type: post
  Operation:
    properties:
      done:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      response:
        description: This is a default description.
        type: post
  RecognitionAudio:
    properties:
      content:
        description: This is a default description.
        type: post
      uri:
        description: This is a default description.
        type: post
  RecognitionConfig:
    properties:
      encoding:
        description: This is a default description.
        type: post
      languageCode:
        description: This is a default description.
        type: post
      maxAlternatives:
        description: This is a default description.
        type: post
      profanityFilter:
        description: This is a default description.
        type: post
      sampleRate:
        description: This is a default description.
        type: post
  SpeechContext:
    properties:
      phrases:
        description: This is a default description.
        type: post
  SpeechRecognitionAlternative:
    properties:
      confidence:
        description: This is a default description.
        type: post
      transcript:
        description: This is a default description.
        type: post
  SpeechRecognitionResult:
    properties:
      alternatives:
        description: This is a default description.
        type: post
  Status:
    properties:
      code:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  SyncRecognizeRequest:
    properties: []
  SyncRecognizeResponse:
    properties:
      results:
        description: This is a default description.
        type: post
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