---
swagger: "2.0"
info:
  title: AWS Polly API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SynthesizeSpeech&k=1:
    get:
      summary: ' Synthesize Speech '
      description: Synthesizes UTF-8 input, plain text or SSML, to a stream of bytes
      operationId: synthesizeSpeech
      parameters:
      - in: query
        name: LexiconNames
        description: List of one or more pronunciation lexicon names you want the
          service to apply      during synthesis
        type: string
      - in: query
        name: OutputFormat
        description: The audio format in which the resulting stream will be encoded
        type: string
      - in: query
        name: SampleRate
        description: The audio frequency specified in Hz
        type: string
      - in: query
        name: Text
        description: Input text to synthesize
        type: string
      - in: query
        name: TextType
        description: Specifies whether the input text is plain text or SSML
        type: string
      - in: query
        name: VoiceId
        description: Voice ID to use for the synthesis
        type: string
      responses:
        200:
          description: OK
      tags:
      - speech
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