---
swagger: "2.0"
info:
  title: Nordea
  description: 'The Nordea''s Open Banking Initiative (OBI) API, offers a safe and
    simple way to try out the upcoming OBI. This API is a sandbox version, and its
    purpose is to make developers familiar with the upcoming OBI production release.
    Moreover, it allows the developers to experiment and build applications which
    use the OBI before its official release. '
  contact:
    name: Open Banking team
  version: 1.0.0
host: api.nordeaopenbanking.com
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/transactions:
    get:
      summary: Get account transactions
      description: Get accounts account transactions
      operationId: transactionsList
      parameters:
      - in: path
        name: accountId
        description: Internal account identifier
      - in: query
        name: continuationKey
        description: Resource listing may return a continuationKey if there's more
          results available
      - in: query
        name: fromDate
        description: List transactions starting from and including this date
      - in: query
        name: language
        description: Preferred language for textual values
      - in: query
        name: toDate
        description: List transactions until and including this date
      responses:
        200:
          description: OK
      tags:
      - accounts
      - account
      - transactions
definitions:
  AccountListResponse:
    properties: []
  ResponseHeader:
    properties:
      creationDateTime:
        description: This is a default description.
        type: get
      httpCode:
        description: This is a default description.
        type: get
      messageIdentification:
        description: This is a default description.
        type: get
  Pagination:
    properties:
      continuationKey:
        description: This is a default description.
        type: get
  AccountList:
    properties:
      accounts:
        description: This is a default description.
        type: get
  AccountInfo:
    properties:
      _id:
        description: This is a default description.
        type: get
      _links:
        description: This is a default description.
        type: get
      accountType:
        description: This is a default description.
        type: get
      availableBalance:
        description: This is a default description.
        type: get
      bookedBalance:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      ownerName:
        description: This is a default description.
        type: get
      product:
        description: This is a default description.
        type: get
      valueDatedBalance:
        description: This is a default description.
        type: get
  Link:
    properties:
      href:
        description: This is a default description.
        type: get
      rel:
        description: This is a default description.
        type: get
  AccountNumber:
    properties:
      _type:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  APIErrorResponse:
    properties: []
  ErrorResponse:
    properties:
      failures:
        description: This is a default description.
        type: get
      httpCode:
        description: This is a default description.
        type: get
  Failure:
    properties:
      code:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  APIRequestEcho:
    properties:
      messageIdentifier:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
  AccountDetailsResponse:
    properties: []
  AccountDetails:
    properties:
      _id:
        description: This is a default description.
        type: get
      _links:
        description: This is a default description.
        type: get
      accountType:
        description: This is a default description.
        type: get
      availableBalance:
        description: This is a default description.
        type: get
      bookedBalance:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      creditLimit:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      latestTransactionBookingDate:
        description: This is a default description.
        type: get
      ownerName:
        description: This is a default description.
        type: get
  BankInfo:
    properties:
      bic:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  TransactionListResponse:
    properties: []
  TransactionList:
    properties:
      _continuationKey:
        description: This is a default description.
        type: get
      _links:
        description: This is a default description.
        type: get
      transactions:
        description: This is a default description.
        type: get
  Transaction:
    properties:
      _type:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      bookingDate:
        description: This is a default description.
        type: get
      creditorMessage:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      transactionId:
        description: This is a default description.
        type: get
      typeDescription:
        description: This is a default description.
        type: get
      valueDate:
        description: This is a default description.
        type: get
  Reference:
    properties:
      _type:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  PaymentResponse:
    properties: []
  Payment:
    properties:
      _id:
        description: This is a default description.
        type: put
      amount:
        description: This is a default description.
        type: put
      currency:
        description: This is a default description.
        type: put
      paymentStatus:
        description: This is a default description.
        type: put
      timestamp:
        description: This is a default description.
        type: put
  PaymentCreditor:
    properties:
      message:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
  PaymentDebtor:
    properties:
      _accountId:
        description: This is a default description.
        type: put
  CreatePaymentRequest:
    properties:
      amount:
        description: This is a default description.
        type: put
      currency:
        description: This is a default description.
        type: put
  PaymentListResponse:
    properties: []
  PaymentList:
    properties:
      _links:
        description: This is a default description.
        type: put
      payments:
        description: This is a default description.
        type: put
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