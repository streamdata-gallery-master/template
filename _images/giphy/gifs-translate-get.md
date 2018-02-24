---
swagger: "2.0"
info:
  title: Giphy
  description: Natively embed all the best features of the world's largest and most
    powerful GIF library into your app.
  termsOfService: https://developers.giphy.com/
  version: v1
host: api.giphy.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gifs/translate:
    get:
      summary: Translate phrase to GIF
      description: The translate API draws on search, but uses the GIPHY `special
        sauce` to handle translating from one vocabulary to another
      operationId: translateGif
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - gifs
      - translate
definitions:
  Gif:
    properties:
      bitly_url:
        description: This is a default description.
        type: get
      content_url:
        description: This is a default description.
        type: get
      create_datetime:
        description: This is a default description.
        type: get
      embded_url:
        description: This is a default description.
        type: get
      featured_tags:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      images:
        description: This is a default description.
        type: get
      import_datetime:
        description: This is a default description.
        type: get
      rating:
        description: This is a default description.
        type: get
      slug:
        description: This is a default description.
        type: get
  Image:
    properties:
      frames:
        description: This is a default description.
        type: get
      height:
        description: This is a default description.
        type: get
      mp4:
        description: This is a default description.
        type: get
      mp4_size:
        description: This is a default description.
        type: get
      size:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
      webp:
        description: This is a default description.
        type: get
      webp_size:
        description: This is a default description.
        type: get
      width:
        description: This is a default description.
        type: get
  Meta:
    properties:
      msg:
        description: This is a default description.
        type: get
      response_id:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
  Pagination:
    properties:
      count:
        description: This is a default description.
        type: get
      offset:
        description: This is a default description.
        type: get
      total_count:
        description: This is a default description.
        type: get
  User:
    properties:
      avatar_url:
        description: This is a default description.
        type: get
      banner_url:
        description: This is a default description.
        type: get
      display_name:
        description: This is a default description.
        type: get
      profile_url:
        description: This is a default description.
        type: get
      twitter:
        description: This is a default description.
        type: get
      username:
        description: This is a default description.
        type: get
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