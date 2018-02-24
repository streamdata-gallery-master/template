---
swagger: "2.0"
info:
  title: AWS Snowball API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateJob&k=1:
    get:
      summary: ' Update Job '
      description: |-
        While a job's JobState value is New, you can update some of
              the information associated with a job
      operationId: updateJob
      parameters:
      - in: query
        name: AddressId
        description: The ID of the updated Address object
        type: string
      - in: query
        name: Description
        description: The updated description of this job's JobMetadata object
        type: string
      - in: query
        name: JobId
        description: The job ID of the job that you want to update, for example        JID123e4567-e89b-12d3-a456-426655440000
        type: string
      - in: query
        name: Notification
        description: The new or updated Notification object
        type: string
      - in: query
        name: Resources
        description: The updated S3Resource object (for a single Amazon S3 bucket
          or key      range), or the updated JobResource object (for multiple buckets
          or key      ranges)
        type: string
      - in: query
        name: RoleARN
        description: The new role Amazon Resource Name (ARN) that you want to associate
          with this job
        type: string
      - in: query
        name: ShippingOption
        description: The updated shipping option value of this job's ShippingDetails      object
        type: string
      - in: query
        name: SnowballCapacityPreference
        description: The updated SnowballCapacityPreference of this job's JobMetadata
          object
        type: string
      responses:
        200:
          description: OK
      tags:
      - jobs
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