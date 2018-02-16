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
  /query?function=BATCH_STOCK_QUOTES:
    get:
      summary: Batch Stock Quotes
      description: The batch stock quotes API enables the querying of multiple stock
        quotes with a single API request, updated realtime
      operationId: getBatchStockQuotes
      parameters:
      - in: query
        name: symbols
        description: Up to 100 stock symbols seperated by comma
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
      - ' Stock Quotes'
definitions: []
---