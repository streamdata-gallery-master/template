---
swagger: "2.0"
info:
  title: Azure Activity Log Alerts API
  version: 2017-03-01-preview
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/microsoft.insights/activityLogAlerts:
    get:
      summary: Activity Log Alerts List By Subscription Id
      description: Get a list of all activity log alerts in a subscription
      operationId: ActivityLogAlerts_ListBySubscriptionId
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - activity log alerts subscription id
definitions:
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
  ActivityLogAlertResource:
    properties: []
  ActivityLogAlertList:
    properties:
      value:
        description: This is a default description.
        type: get
  ActivityLogAlert:
    properties:
      scopes:
        description: This is a default description.
        type: get
      enabled:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
  ActivityLogAlertAllOfCondition:
    properties:
      allOf:
        description: This is a default description.
        type: get
  ActivityLogAlertLeafCondition:
    properties:
      field:
        description: This is a default description.
        type: get
      equals:
        description: This is a default description.
        type: get
  ActivityLogAlertActionList:
    properties:
      actionGroups:
        description: This is a default description.
        type: get
  ActivityLogAlertActionGroup:
    properties:
      actionGroupId:
        description: This is a default description.
        type: get
  ErrorResponse:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  ActivityLogAlertResourcePatch:
    properties: []
  ActivityLogAlertPatch:
    properties:
      enabled:
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