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
  /?Action=CreateJob&k=1:
    get:
      summary: ' Create Job '
      description: |-
        Creates a job to import or export data between Amazon S3 and your on-premises data
              center
      operationId: createJob
      parameters:
      - in: query
        name: AddressId
        description: The ID for the address that you want the Snowball shipped to
        type: string
      - in: query
        name: ClusterId
        description: The ID of a cluster
        type: string
      - in: query
        name: Description
        description: Defines an optional description of this specific job, for example
          Important        Photos 2016-08-11
        type: string
      - in: query
        name: JobType
        description: Defines the type of job that you're creating
        type: string
      - in: query
        name: KmsKeyARN
        description: The KmsKeyARN that you want to associate with this job
        type: string
      - in: query
        name: Notification
        description: Defines the Amazon Simple Notification Service (Amazon SNS) notification
          settings for      this job
        type: string
      - in: query
        name: Resources
        description: Defines the Amazon S3 buckets associated with this job
        type: string
      - in: query
        name: RoleARN
        description: The RoleARN that you want to associate with this job
        type: string
      - in: query
        name: ShippingOption
        description: The shipping speed for this job
        type: string
      - in: query
        name: SnowballCapacityPreference
        description: If your job is being created in one of the US regions, you have
          the option of      specifying what size Snowball you'd like for this job
        type: string
      - in: query
        name: SnowballType
        description: The type of AWS Snowball appliance to use for this job
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