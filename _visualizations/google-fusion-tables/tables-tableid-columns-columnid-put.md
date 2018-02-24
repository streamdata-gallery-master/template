---
swagger: "2.0"
info:
  title: Fusion Tables
  description: API for working with Fusion Tables data.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /fusiontables/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tables/{tableId}/columns/{columnId}:
    put:
      summary: Update Column
      description: Updates the name or type of an existing column
      operationId: fusiontables.column.update
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: columnId
        description: Name or identifier for the column that is being updated
      - in: path
        name: tableId
        description: Table for which the column is being updated
      responses:
        200:
          description: OK
      tags:
      - column
definitions:
  Bucket:
    properties:
      color:
        description: This is a default description.
        type: put
      icon:
        description: This is a default description.
        type: put
      max:
        description: This is a default description.
        type: put
      min:
        description: This is a default description.
        type: put
      opacity:
        description: This is a default description.
        type: put
      weight:
        description: This is a default description.
        type: put
  Column:
    properties:
      baseColumn:
        description: This is a default description.
        type: put
      columnId:
        description: This is a default description.
        type: put
      columnJsonSchema:
        description: This is a default description.
        type: put
      columnPropertiesJson:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      formatPattern:
        description: This is a default description.
        type: put
      graphPredicate:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  ColumnList:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
      totalItems:
        description: This is a default description.
        type: put
  Geometry:
    properties:
      geometries:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  Import:
    properties:
      kind:
        description: This is a default description.
        type: put
      numRowsReceived:
        description: This is a default description.
        type: put
  Line:
    properties:
      coordinates:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  LineStyle:
    properties:
      strokeColor:
        description: This is a default description.
        type: put
      strokeOpacity:
        description: This is a default description.
        type: put
      strokeWeight:
        description: This is a default description.
        type: put
  Point:
    properties:
      coordinates:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  PointStyle:
    properties:
      iconName:
        description: This is a default description.
        type: put
  Polygon:
    properties:
      coordinates:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  PolygonStyle:
    properties:
      fillColor:
        description: This is a default description.
        type: put
      fillOpacity:
        description: This is a default description.
        type: put
      strokeColor:
        description: This is a default description.
        type: put
      strokeOpacity:
        description: This is a default description.
        type: put
      strokeWeight:
        description: This is a default description.
        type: put
  Sqlresponse:
    properties:
      columns:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      rows:
        description: This is a default description.
        type: put
  StyleFunction:
    properties:
      buckets:
        description: This is a default description.
        type: put
      columnName:
        description: This is a default description.
        type: put
      gradient:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  StyleSetting:
    properties:
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      styleId:
        description: This is a default description.
        type: put
      tableId:
        description: This is a default description.
        type: put
  StyleSettingList:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
      totalItems:
        description: This is a default description.
        type: put
  Table:
    properties:
      attribution:
        description: This is a default description.
        type: put
      attributionLink:
        description: This is a default description.
        type: put
      baseTableIds:
        description: This is a default description.
        type: put
      columnPropertiesJsonSchema:
        description: This is a default description.
        type: put
      columns:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      isExportable:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      sql:
        description: This is a default description.
        type: put
  TableList:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  Task:
    properties:
      kind:
        description: This is a default description.
        type: put
      progress:
        description: This is a default description.
        type: put
      started:
        description: This is a default description.
        type: put
      taskId:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  TaskList:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
      totalItems:
        description: This is a default description.
        type: put
  Template:
    properties:
      automaticColumnNames:
        description: This is a default description.
        type: put
      body:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      tableId:
        description: This is a default description.
        type: put
      templateId:
        description: This is a default description.
        type: put
  TemplateList:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
      totalItems:
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