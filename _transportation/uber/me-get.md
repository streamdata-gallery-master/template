---
swagger: "2.0"
info:
  title: Uber API
  description: Move your app forward with the Uber API
  version: 1.0.0
host: api.uber.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me:
    get:
      summary: User Profile
      description: The User Profile endpoint returns information about the Uber user
        that has authorized with the application
      operationId: the-user-profile-endpoint-returns-information-about-the-uber-user-that-has-authorized-with-the-appli
      responses:
        200:
          description: OK
      tags:
      - transportation
definitions:
  Product:
    properties:
      product_id:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      display_name:
        description: This is a default description.
        type: get
      capacity:
        description: This is a default description.
        type: get
      image:
        description: This is a default description.
        type: get
  ProductList:
    properties:
      products:
        description: This is a default description.
        type: get
  PriceEstimate:
    properties:
      product_id:
        description: This is a default description.
        type: get
      currency_code:
        description: This is a default description.
        type: get
      display_name:
        description: This is a default description.
        type: get
      estimate:
        description: This is a default description.
        type: get
      low_estimate:
        description: This is a default description.
        type: get
      high_estimate:
        description: This is a default description.
        type: get
      surge_multiplier:
        description: This is a default description.
        type: get
  Profile:
    properties:
      first_name:
        description: This is a default description.
        type: get
      last_name:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      picture:
        description: This is a default description.
        type: get
      promo_code:
        description: This is a default description.
        type: get
  Activity:
    properties:
      uuid:
        description: This is a default description.
        type: get
  Activities:
    properties:
      offset:
        description: This is a default description.
        type: get
      limit:
        description: This is a default description.
        type: get
      count:
        description: This is a default description.
        type: get
      history:
        description: This is a default description.
        type: get
  Error:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      fields:
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