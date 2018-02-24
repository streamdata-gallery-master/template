---
swagger: "2.0"
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RunJobFlow&k=1:
    get:
      summary: ' Run Job Flow '
      description: RunJobFlow creates and starts running a new job flow
      operationId: runJobFlow
      parameters:
      - in: query
        name: AdditionalInfo
        description: A JSON string for selecting additional features
        type: string
      - in: query
        name: AmiVersion
        description: Note
        type: string
      - in: query
        name: Applications
        description: Note
        type: string
      - in: query
        name: AutoScalingRole
        description: An IAM role for automatic scaling policies
        type: string
      - in: query
        name: BootstrapActions
        description: A list of bootstrap actions that will be run before Hadoop is
          started on the cluster nodes
        type: string
      - in: query
        name: Configurations
        description: Note
        type: string
      - in: query
        name: Instances
        description: A specification of the number and type of Amazon EC2 instances
          on which to run the job flow
        type: string
      - in: query
        name: JobFlowRole
        description: Also called instance profile and EC2 role
        type: string
      - in: query
        name: LogUri
        description: The location in Amazon S3 to write the log files of the job flow
        type: string
      - in: query
        name: Name
        description: The name of the job flow
        type: string
      - in: query
        name: NewSupportedProducts
        description: Note
        type: string
      - in: query
        name: ReleaseLabel
        description: Note
        type: string
      - in: query
        name: ScaleDownBehavior
        description: Specifies the way that individual Amazon EC2 instances terminate
          when an automatic scale-in activity occurs or an instance group is resized
        type: string
      - in: query
        name: SecurityConfiguration
        description: The name of a security configuration to apply to the cluster
        type: string
      - in: query
        name: ServiceRole
        description: The IAM role that will be assumed by the Amazon EMR service to
          access AWS resources on your behalf
        type: string
      - in: query
        name: Steps
        description: A list of steps to be executed by the job flow
        type: string
      - in: query
        name: SupportedProducts
        description: Note
        type: string
      - in: query
        name: Tags
        description: A list of tags to associate with a cluster and propagate to Amazon
          EC2 instances
        type: string
      - in: query
        name: VisibleToAllUsers
        description: Whether the job flow is visible to all IAM users of the AWS account
          associated with the job flow
        type: string
      responses:
        200:
          description: OK
      tags:
      - job flows
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