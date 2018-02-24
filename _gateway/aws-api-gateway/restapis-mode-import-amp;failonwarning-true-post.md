---
swagger: "2.0"
info:
  title: AWS API Gateway API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapis?mode=import&amp;failonwarning=true:
    post:
      summary: Restapi Import
      description: Creates an API from an external API definition
      operationId: restapiImport
      parameters:
      - in: header
        name: '&quot;$ref&quot;'
        type: string
      - in: header
        name: '&quot;/&quot;'
        type: string
      - in: header
        name: '&quot;200&quot;'
        type: string
      - in: header
        name: '&quot;application/json&quot;'
        type: string
      - in: header
        name: '&quot;basePath&quot;'
        type: string
      - in: header
        name: '&quot;consumes&quot;'
        type: string
      - in: header
        name: '&quot;Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;default&quot;'
        type: string
      - in: header
        name: '&quot;definitions&quot;'
        type: string
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: '&quot;Empty&quot;'
        type: string
      - in: header
        name: '&quot;get&quot;'
        type: string
      - in: header
        name: '&quot;headers&quot;'
        type: string
      - in: header
        name: '&quot;host&quot;'
        type: string
      - in: header
        name: '&quot;httpMethod&quot;'
        type: string
      - in: header
        name: '&quot;info&quot;'
        type: string
      - in: header
        name: '&quot;integration.request.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;method.response.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;passthroughBehavior&quot;'
        type: string
      - in: header
        name: '&quot;paths&quot;'
        type: string
      - in: header
        name: '&quot;produces&quot;'
        type: string
      - in: header
        name: '&quot;requestParameters&quot;'
        type: string
      - in: header
        name: '&quot;requestTemplates&quot;'
        type: string
      - in: header
        name: '&quot;responseParameters&quot;'
        type: string
      - in: header
        name: '&quot;responses&quot;'
        type: string
      - in: header
        name: '&quot;responseTemplates&quot;'
        type: string
      - in: header
        name: '&quot;schema&quot;'
        type: string
      - in: header
        name: '&quot;schemes&quot;'
        type: string
      - in: header
        name: '&quot;statusCode&quot;'
        type: string
      - in: header
        name: '&quot;swagger&quot;'
        type: string
      - in: header
        name: '&quot;title&quot;'
        type: string
      - in: header
        name: '&quot;type&quot;'
        type: string
      - in: header
        name: '&quot;x-amazon-apigateway-integration&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - api
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