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
  /?Action=CreateReplicationGroup&k=1:
    get:
      summary: ' Create Replication Group '
      description: Creates a Redis (cluster mode disabled) or a Redis (cluster mode
        enabled) replication group
      operationId: createReplicationGroup
      parameters:
      - in: query
        name: AuthToken
        description: Reserved parameter
        type: string
      - in: query
        name: AutomaticFailoverEnabled
        description: Specifies whether a read-only replica is automatically promoted
          to read/write primary if the existing primary fails
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: This parameter is currently disabled
        type: string
      - in: query
        name: CacheNodeType
        description: The compute and memory capacity of the nodes in the node group
          (shard)
        type: string
      - in: query
        name: CacheParameterGroupName
        description: The name of the parameter group to associate with this replication
          group
        type: string
      - in: query
        name: CacheSecurityGroupNames.CacheSecurityGroupName.N
        description: A list of cache security group names to associate with this replication
          group
        type: string
      - in: query
        name: CacheSubnetGroupName
        description: The name of the cache subnet group to be used for the replication
          group
        type: string
      - in: query
        name: Engine
        description: The name of the cache engine to be used for the cache clusters
          in this replication group
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the cache engine to be used for the cache
          clusters in this replication group
        type: string
      - in: query
        name: NodeGroupConfiguration.NodeGroupConfiguration.N
        description: A list of node group (shard) configuration options
        type: string
      - in: query
        name: NotificationTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon Simple Notification
          Service (SNS) topic to which notifications are sent
        type: string
      - in: query
        name: NumCacheClusters
        description: The number of clusters this replication group initially has
        type: string
      - in: query
        name: NumNodeGroups
        description: An optional parameter that specifies the number of node groups
          (shards) for this Redis (cluster mode enabled) replication group
        type: string
      - in: query
        name: Port
        description: The port number on which each member of the replication group
          accepts connections
        type: string
      - in: query
        name: PreferredCacheClusterAZs.AvailabilityZone.N
        description: A list of EC2 Availability Zones in which the replication group's
          cache clusters are created
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: Specifies the weekly time range during which maintenance    on
          the cache cluster is performed
        type: string
      - in: query
        name: PrimaryClusterId
        description: The identifier of the cache cluster that serves as the primary
          for this replication            group
        type: string
      - in: query
        name: ReplicasPerNodeGroup
        description: An optional parameter that specifies the number of replica nodes
          in each node group (shard)
        type: string
      - in: query
        name: ReplicationGroupDescription
        description: A user-created description for the replication group
        type: string
      - in: query
        name: ReplicationGroupId
        description: The replication group identifier
        type: string
      - in: query
        name: SecurityGroupIds.SecurityGroupId.N
        description: One or more Amazon VPC security groups associated with this replication
          group
        type: string
      - in: query
        name: SnapshotArns.SnapshotArn.N
        description: A list of Amazon Resource Names (ARN) that uniquely identify           the
          Redis RDB snapshot files stored in Amazon S3
        type: string
      - in: query
        name: SnapshotName
        description: The name of a snapshot from which to restore data into the new
          replication group
        type: string
      - in: query
        name: SnapshotRetentionLimit
        description: The number of days for which ElastiCache retains automatic snapshots
          before deleting them
        type: string
      - in: query
        name: SnapshotWindow
        description: The daily time range (in UTC) during which ElastiCache begins
          taking a daily snapshot of your node group (shard)
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of cost allocation tags to be added to this resource
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