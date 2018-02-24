---
swagger: "2.0"
info:
  title: Enterprise Apps Reseller
  description: Creates and manages your customers and their subscriptions.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /apps/reseller/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers/{customerId}/subscriptions/{subscriptionId}/changeSeats:
    post:
      summary: Update Suscription License
      description: Update a subscription's user license settings
      operationId: reseller.subscriptions.changeSeats
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
        description: Either the customer's primary domain name or the customer's unique
          identifier
      - in: path
        name: subscriptionId
        description: This is a required property
      responses:
        200:
          description: OK
      tags:
      - license
definitions:
  Address:
    properties:
      addressLine1:
        description: This is a default description.
        type: parameters
      addressLine2:
        description: This is a default description.
        type: parameters
      addressLine3:
        description: This is a default description.
        type: parameters
      contactName:
        description: This is a default description.
        type: parameters
      countryCode:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      locality:
        description: This is a default description.
        type: parameters
      organizationName:
        description: This is a default description.
        type: parameters
      postalCode:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
  ChangePlanRequest:
    properties:
      dealCode:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      planName:
        description: This is a default description.
        type: parameters
      purchaseOrderId:
        description: This is a default description.
        type: parameters
  Customer:
    properties:
      alternateEmail:
        description: This is a default description.
        type: parameters
      customerDomain:
        description: This is a default description.
        type: parameters
      customerDomainVerified:
        description: This is a default description.
        type: parameters
      customerId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      phoneNumber:
        description: This is a default description.
        type: parameters
      resourceUiUrl:
        description: This is a default description.
        type: parameters
  RenewalSettings:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      renewalType:
        description: This is a default description.
        type: parameters
  ResellernotifyGetwatchdetailsResponse:
    properties:
      serviceAccountEmailAddresses:
        description: This is a default description.
        type: parameters
      topicName:
        description: This is a default description.
        type: parameters
  ResellernotifyResource:
    properties:
      topicName:
        description: This is a default description.
        type: parameters
  Seats:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      licensedNumberOfSeats:
        description: This is a default description.
        type: parameters
      maximumNumberOfSeats:
        description: This is a default description.
        type: parameters
      numberOfSeats:
        description: This is a default description.
        type: parameters
  Subscription:
    properties:
      billingMethod:
        description: This is a default description.
        type: parameters
      creationTime:
        description: This is a default description.
        type: parameters
      customerDomain:
        description: This is a default description.
        type: parameters
      customerId:
        description: This is a default description.
        type: parameters
      dealCode:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      plan:
        description: This is a default description.
        type: parameters
      purchaseOrderId:
        description: This is a default description.
        type: parameters
      resourceUiUrl:
        description: This is a default description.
        type: parameters
      skuId:
        description: This is a default description.
        type: parameters
  Subscriptions:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      subscriptions:
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