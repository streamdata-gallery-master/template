---
swagger: "2.0"
info:
  title: Admin Reports
  description: Fetches reports for the administrators of Google Apps customers about
    the usage, collaboration, security, and risk for their users.
  contact:
    name: Google
    url: https://google.com
  version: reports_v1
host: www.googleapis.com
basePath: /admin/reports/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /usage/users/{userKey}/dates/{date}:
    get:
      summary: Get User Report by Date
      description: Retrieves a report which is a collection of properties / statistics
        for a set of users
      operationId: reports.userUsageReport.get
      parameters:
      - in: query
        name: customerId
        description: Represents the customer for which the data is to be fetched
      - in: path
        name: date
        description: Represents the date in yyyy-mm-dd format for which the data is
          to be fetched
      - in: query
        name: filters
        description: Represents the set of filters including parameter operator value
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Token to specify next page
      - in: query
        name: parameters
        description: Represents the application name, parameter name pairs to fetch
          in csv as app_name1:param_name1, app_name2:param_name2
      - in: path
        name: userKey
        description: Represents the profile id or the user email for which the data
          should be filtered
      responses:
        200:
          description: OK
      tags:
      - report
definitions:
  Activities:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  Activity:
    properties:
      actor:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      events:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      ipAddress:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      ownerDomain:
        description: This is a default description.
        type: parameters
  Channel:
    properties:
      address:
        description: This is a default description.
        type: parameters
      expiration:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      params:
        description: This is a default description.
        type: parameters
      payload:
        description: This is a default description.
        type: parameters
      resourceId:
        description: This is a default description.
        type: parameters
      resourceUri:
        description: This is a default description.
        type: parameters
      token:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  UsageReport:
    properties:
      date:
        description: This is a default description.
        type: parameters
      entity:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      parameters:
        description: This is a default description.
        type: parameters
  UsageReports:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      usageReports:
        description: This is a default description.
        type: parameters
      warnings:
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