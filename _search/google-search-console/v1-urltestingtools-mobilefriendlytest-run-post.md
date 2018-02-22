---
swagger: "2.0"
info:
  title: Google Search Console URL Testing Tools
  description: Provides tools for running validation tests against single URLs
  contact:
    name: Google
    url: https://google.com
  version: v1
host: searchconsole.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/urlTestingTools/mobileFriendlyTest:run:
    post:
      summary: Run Mobile Friendly Test
      description: Runs Mobile-Friendly Test for a given URL
      operationId: searchconsole.urlTestingTools.mobileFriendlyTest.run
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - test
definitions:
  BlockedResource:
    properties:
      url:
        description: This is a default description.
        type: post
  Image:
    properties:
      data:
        description: This is a default description.
        type: post
      mimeType:
        description: This is a default description.
        type: post
  MobileFriendlyIssue:
    properties:
      rule:
        description: This is a default description.
        type: post
  ResourceIssue:
    properties: []
  RunMobileFriendlyTestRequest:
    properties:
      requestScreenshot:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
  RunMobileFriendlyTestResponse:
    properties:
      mobileFriendliness:
        description: This is a default description.
        type: post
      mobileFriendlyIssues:
        description: This is a default description.
        type: post
      resourceIssues:
        description: This is a default description.
        type: post
  TestStatus:
    properties:
      details:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
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