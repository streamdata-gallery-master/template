---
swagger: "2.0"
info:
  title: Microsoft.ResourceHealth
  description: The Resource Health Client.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{resourceUri}/providers/Microsoft.ResourceHealth/availabilityStatuses:
    get:
      summary: Availability Statuses List
      description: Lists the historical availability statuses for a single resource
      operationId: AvailabilityStatuses_List
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceUri
        description: The fully qualified ID of the resource, including the resource
          name and resource type
      responses:
        200:
          description: OK
      tags:
      - availability statuses
definitions:
  availabilityStatusListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  availabilityStatus:
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
      properties:
        description: This is a default description.
        type: get
  recommendedAction:
    properties:
      action:
        description: This is a default description.
        type: get
      actionUrl:
        description: This is a default description.
        type: get
      actionUrlText:
        description: This is a default description.
        type: get
  serviceImpactingEvent:
    properties:
      eventStartTime:
        description: This is a default description.
        type: get
      eventStatusLastModifiedTime:
        description: This is a default description.
        type: get
      correlationId:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      incidentProperties:
        description: This is a default description.
        type: get
  operationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  operation:
    properties:
      name:
        description: This is a default description.
        type: get
      display:
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
      details:
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