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
  /?Action=CreateCluster&k=1:
    get:
      summary: ' Create Cluster '
      description: Creates an empty cluster
      operationId: createCluster
      parameters:
      - in: query
        name: AddressId
        description: The ID for the address that you want the cluster shipped to
        type: string
      - in: query
        name: Description
        description: An optional description of this specific cluster, for example
          Environmental Data        Cluster-01
        type: string
      - in: query
        name: JobType
        description: The type of job for this cluster
        type: string
      - in: query
        name: KmsKeyARN
        description: The KmsKeyARN value that you want to associate with this cluster
        type: string
      - in: query
        name: Notification
        description: The Amazon Simple Notification Service (Amazon SNS) notification
          settings for this      cluster
        type: string
      - in: query
        name: Resources
        description: The resources associated with the cluster job
        type: string
      - in: query
        name: RoleARN
        description: The RoleARN that you want to associate with this cluster
        type: string
      - in: query
        name: ShippingOption
        description: The shipping speed for each node in this cluster
        type: string
      - in: query
        name: SnowballType
        description: The type of AWS Snowball appliance to use for this cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - clusters
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