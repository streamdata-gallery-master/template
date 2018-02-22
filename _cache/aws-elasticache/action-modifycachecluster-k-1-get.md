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
  /?Action=ModifyCacheCluster&k=1:
    get:
      summary: ' Modify Cache Cluster '
      description: Modifies the settings for a cache cluster
      operationId: modifyCacheCluster
      parameters:
      - in: query
        name: ApplyImmediately
        description: If true, this parameter causes the modifications in this request
          and any            pending modifications to be applied, asynchronously and
          as soon as possible, regardless            of the PreferredMaintenanceWindow
          setting for the cache cluster
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: This parameter is currently disabled
        type: string
      - in: query
        name: AZMode
        description: Specifies whether the new nodes in this Memcached cache cluster
          are all created in a             single Availability Zone or created across
          multiple Availability Zones
        type: string
      - in: query
        name: CacheClusterId
        description: The cache cluster identifier
        type: string
      - in: query
        name: CacheNodeIdsToRemove.CacheNodeId.N
        description: A list of cache node IDs to be removed
        type: string
      - in: query
        name: CacheNodeType
        description: A valid cache node type that you want to scale this cache cluster
          up to
        type: string
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to apply to this cache
          cluster
        type: string
      - in: query
        name: CacheSecurityGroupNames.CacheSecurityGroupName.N
        description: A list of cache security group names to authorize on this cache
          cluster
        type: string
      - in: query
        name: EngineVersion
        description: The upgraded version of the cache engine to be run on the cache
          nodes
        type: string
      - in: query
        name: NewAvailabilityZones.PreferredAvailabilityZone.N
        description: The list of Availability Zones where the new Memcached cache
          nodes are created
        type: string
      - in: query
        name: NotificationTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic to which
          notifications are sent
        type: string
      - in: query
        name: NotificationTopicStatus
        description: The status of the Amazon SNS notification topic
        type: string
      - in: query
        name: NumCacheNodes
        description: The number of cache nodes that the cache cluster should have
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: Specifies the weekly time range during which maintenance   on
          the cluster is performed
        type: string
      - in: query
        name: SecurityGroupIds.SecurityGroupId.N
        description: Specifies the VPC Security Groups associated with the cache cluster
        type: string
      - in: query
        name: SnapshotRetentionLimit
        description: The number of days for which ElastiCache retains automatic cache
          cluster snapshots before            deleting them
        type: string
      - in: query
        name: SnapshotWindow
        description: The daily time range (in UTC) during which ElastiCache  begins
          taking a daily snapshot of            your cache cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - cache clusters
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