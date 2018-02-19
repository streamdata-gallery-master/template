---
swagger: "2.0"
info:
  title: LinkedIn
  description: Bring user profiles and professional networks to your apps.
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/{id}/historical-follow-statistics:
    get:
      summary: Get Companies Historical Follow Statistics
      description: Get companies  historical follow statistics
      operationId: getCompaniesHistoricalFollowStatistics
      responses:
        200:
          description: OK
      tags:
      - companies
      - ""
      - historical
      - follow
      - statistics
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