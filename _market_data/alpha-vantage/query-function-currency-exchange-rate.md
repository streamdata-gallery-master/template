---
swagger: "2.0"
info:
  title: Alpha Vantage
  description: 'Alpha Vantage APIs are grouped into four categories: (1) Stock Time
    Series Data, (2) Physical and Digital/Crypto Currencies (e.g., Bitcoin), (3) Stock
    Technical Indicators, and (4) Sector Performances. All APIs are realtime: the
    latest data points are derived from the current trading day. '
  version: 1.0.0
host: www.alphavantage.co
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query?function=CURRENCY_EXCHANGE_RATE:
    get:
      summary: Currency Exchange Rates
      description: Realtime currency exchange rates for physical and digital currencies
      operationId: getCurrencyExchangeRates
      parameters:
      - in: query
        name: from_currency
        description: The currency you would like to get the exchange rate for
        type: string
        format: string
      - in: query
        name: to_currency
        description: The destination currency for the exchange rate
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Currency
      - ' Exchange Rates'
definitions: []
---