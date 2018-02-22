---
swagger: "2.0"
info:
  title: Translate
  description: Translates text from one language to another.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /language/translate
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/languages:
    get:
      summary: Get Languages
      description: List the source/target languages supported by the API
      operationId: language.languages.list
      parameters:
      - in: query
        name: target
        description: the language and collation in which the localized results should
          be returned
      responses:
        200:
          description: OK
      tags:
      - language
definitions:
  DetectionsListResponse:
    properties:
      detections:
        description: This is a default description.
        type: parameters
  LanguagesListResponse:
    properties:
      languages:
        description: This is a default description.
        type: parameters
  LanguagesResource:
    properties:
      language:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  TranslationsListResponse:
    properties:
      translations:
        description: This is a default description.
        type: parameters
  TranslationsResource:
    properties:
      detectedSourceLanguage:
        description: This is a default description.
        type: parameters
      translatedText:
        description: This is a default description.
        type: parameters
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