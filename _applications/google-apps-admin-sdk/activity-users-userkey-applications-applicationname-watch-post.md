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
  /activity/users/{userKey}/applications/{applicationName}/watch:
    post:
      summary: Change Activity
      description: Push changes to activities
      operationId: reports.activities.watch
      parameters:
      - in: query
        name: actorIpAddress
        description: IP Address of host where the event was performed
      - in: path
        name: applicationName
        description: Application name for which the events are to be retrieved
      - in: query
        name: customerId
        description: Represents the customer for which the data is to be fetched
      - in: query
        name: endTime
        description: Return events which occured at or before this time
      - in: query
        name: eventName
        description: Name of the event being queried
      - in: query
        name: filters
        description: Event parameters in the form [parameter1 name][operator][parameter1
          value],[parameter2 name][operator][parameter2 value],
      - in: query
        name: maxResults
        description: Number of activity records to be shown in each page
      - in: query
        name: pageToken
        description: Token to specify next page
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: startTime
        description: Return events which occured at or after this time
      - in: path
        name: userKey
        description: Represents the profile id or the user email for which the data
          should be filtered
      responses:
        200:
          description: OK
      tags:
      - activities
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