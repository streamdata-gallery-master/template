---
swagger: "2.0"
info:
  title: Standard Chartered
  description: Standard Chartered PLC is a British multinational banking and financial
    services company headquartered in London, England. It operates a network of more
    than 1,200 branches and outlets (including subsidiaries, associates and joint
    ventures) across more than 70 countries and employs around 87,000 people. It is
    a universal bank with operations in consumer, corporate and institutional banking,
    and treasury services. Despite its UK base, it does not conduct retail banking
    in the UK, and around 90% of its profits come from Asia, Africa and the Middle
    East.
  termsOfService: https://www.sc.com/terms-and-conditions
  contact:
    name: Steve Spicer
    url: https://www.sc.com
    email: steven.spicer@sc.com
  version: 1.0.0
host: developer.sc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cib/service/s2b/api/v1/banks/scb/reference/default/holiday-calendar/currency/{currency}:
    get:
      summary: Holiday Calendar Inquiry (Currency)
      description: "The \u201CGetHolidayCalendar\u201D API returns list of holidays
        applicable for the specified combination of:\n<ul><li>Currency</li><li>Date
        Range</li></lu>"
      operationId: getCibServiceS2bApiV1BanksScbReferenceDefaultHolayCalendarCurrencyCurrency
      parameters:
      - in: path
        name: currency
      - in: query
        name: endDate
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - cib
      - service
      - s2b
      - api
      - v1
      - banks
      - scb
      - reference
      - default
      - holay
      - calendar
      - currency
      - currency
definitions:
  OpenApiAccount:
    properties:
      id:
        description: This is a default description.
        type: get
      label:
        description: This is a default description.
        type: get
      number:
        description: This is a default description.
        type: get
      owners:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      swift_bic:
        description: This is a default description.
        type: get
      bank_id:
        description: This is a default description.
        type: get
      iban:
        description: This is a default description.
        type: get
  OpenApiAccountBalance:
    properties:
      currency:
        description: This is a default description.
        type: get
      lastUpdated:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
  OpenApiAccountOwner:
    properties:
      id:
        description: This is a default description.
        type: get
      provider:
        description: This is a default description.
        type: get
      display_name:
        description: This is a default description.
        type: get
  OpenApiAddress:
    properties:
      line_1:
        description: This is a default description.
        type: get
      line_2:
        description: This is a default description.
        type: get
      line_3:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      postcode:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
  OpenApiBankBranch:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      swiftCode:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      routingCode:
        description: This is a default description.
        type: get
  OpenApiHoliday:
    properties:
      description:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
  OpenApiHolidays:
    properties:
      holidays:
        description: This is a default description.
        type: get
  OpenApiLicense:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  OpenApiMeta:
    properties: []
  customer:
    properties:
      customerId:
        description: This is a default description.
        type: get
      customerName:
        description: This is a default description.
        type: get
      customerBookingLocation:
        description: This is a default description.
        type: get
      customerDomicileCountry:
        description: This is a default description.
        type: get
      limits:
        description: This is a default description.
        type: get
      transactions:
        description: This is a default description.
        type: get
  transactionList:
    properties:
      customerId:
        description: This is a default description.
        type: get
      customerName:
        description: This is a default description.
        type: get
      updateAsofTime:
        description: This is a default description.
        type: get
      transactionsInProgress:
        description: This is a default description.
        type: get
      releasedTransactions:
        description: This is a default description.
        type: get
  transaction:
    properties:
      transactionsCustomerId:
        description: This is a default description.
        type: get
      transactionCustomerName:
        description: This is a default description.
        type: get
      updateAsofTime:
        description: This is a default description.
        type: get
      transactionsInProgress:
        description: This is a default description.
        type: get
      releasedTransactions:
        description: This is a default description.
        type: get
  limits:
    properties:
      customerLimitDetails:
        description: This is a default description.
        type: get
      coBorrowerLimitDetails:
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