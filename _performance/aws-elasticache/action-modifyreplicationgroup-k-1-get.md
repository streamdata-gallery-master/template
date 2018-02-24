---
swagger: "2.0"
info:
  title: AWS ElastiCache API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyReplicationGroup&k=1:
    get:
      summary: ' Modify Replication Group '
      description: Modifies the settings for a replication group
      operationId: modifyReplicationGroup
      parameters:
      - in: query
        name: ApplyImmediately
        description: If true, this parameter causes the modifications in this request
          and any            pending modifications to be applied, asynchronously and
          as soon as possible, regardless            of the PreferredMaintenanceWindow
          setting for the replication group
        type: string
      - in: query
        name: AutomaticFailoverEnabled
        description: Determines whether a read replica is automatically promoted to
          read/write primary if the existing primary encounters a failure
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: This parameter is currently disabled
        type: string
      - in: query
        name: CacheNodeType
        description: A valid cache node type that you want to scale this replication
          group to
        type: string
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to apply to all of the
          clusters in this replication group
        type: string
      - in: query
        name: CacheSecurityGroupNames.CacheSecurityGroupName.N
        description: A list of cache security group names to authorize for the clusters
          in this replication group
        type: string
      - in: query
        name: EngineVersion
        description: The upgraded version of the cache engine to be run on the cache
          clusters in the replication group
        type: string
      - in: query
        name: NotificationTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic to which
          notifications are sent
        type: string
      - in: query
        name: NotificationTopicStatus
        description: The status of the Amazon SNS notification topic for the replication
          group
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: Specifies the weekly time range during which maintenance   on
          the cluster is performed
        type: string
      - in: query
        name: PrimaryClusterId
        description: For replication groups with a single primary,             if
          this parameter is specified, ElastiCache promotes the specified cluster
          in the specified replication group to the primary role
        type: string
      - in: query
        name: ReplicationGroupDescription
        description: A description for the replication group
        type: string
      - in: query
        name: ReplicationGroupId
        description: The identifier of the replication group to modify
        type: string
      - in: query
        name: SecurityGroupIds.SecurityGroupId.N
        description: Specifies the VPC Security Groups associated with the cache clusters
          in the replication group
        type: string
      - in: query
        name: SnapshotRetentionLimit
        description: The number of days for which ElastiCache retains automatic node
          group (shard) snapshots before            deleting them
        type: string
      - in: query
        name: SnapshottingClusterId
        description: The cache cluster ID that is used as the daily snapshot source
          for the replication group
        type: string
      - in: query
        name: SnapshotWindow
        description: The daily time range (in UTC) during which ElastiCache  begins
          taking a daily snapshot of            the node group (shard) specified by
          SnapshottingClusterId
        type: string
      responses:
        200:
          description: OK
      tags:
      - replication groups
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