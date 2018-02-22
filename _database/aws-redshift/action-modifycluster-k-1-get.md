---
swagger: "2.0"
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyCluster&k=1:
    get:
      summary: ' Modify Cluster '
      description: Modifies the settings for a cluster
      operationId: modifyCluster
      parameters:
      - in: query
        name: AllowVersionUpgrade
        description: If true, major version upgrades will be applied automatically
          to the            cluster during the maintenance window
        type: string
      - in: query
        name: AutomatedSnapshotRetentionPeriod
        description: The number of days that automated snapshots are retained
        type: string
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster to be modified
        type: string
      - in: query
        name: ClusterParameterGroupName
        description: The name of the cluster parameter group to apply to this cluster
        type: string
      - in: query
        name: ClusterSecurityGroups.ClusterSecurityGroupName.N
        description: A list of cluster security groups to be authorized on this cluster
        type: string
      - in: query
        name: ClusterType
        description: The new cluster type
        type: string
      - in: query
        name: ClusterVersion
        description: The new version number of the Amazon Redshift engine to upgrade
          to
        type: string
      - in: query
        name: ElasticIp
        description: The Elastic IP (EIP) address for the cluster
        type: string
      - in: query
        name: EnhancedVpcRouting
        description: An option that specifies whether to create the cluster with enhanced
          VPC routing            enabled
        type: string
      - in: query
        name: HsmClientCertificateIdentifier
        description: Specifies the name of the HSM client certificate the Amazon Redshift
          cluster uses to            retrieve the data encryption keys stored in an
          HSM
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: Specifies the name of the HSM configuration that contains the
          information the            Amazon Redshift cluster can use to retrieve and
          store keys in an HSM
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the cluster master user
        type: string
      - in: query
        name: NewClusterIdentifier
        description: The new identifier for the cluster
        type: string
      - in: query
        name: NodeType
        description: The new node type of the cluster
        type: string
      - in: query
        name: NumberOfNodes
        description: The new number of nodes of the cluster
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which system maintenance
          can occur, if            necessary
        type: string
      - in: query
        name: PubliclyAccessible
        description: If true, the cluster can be accessed from a public network
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of virtual private cloud (VPC) security groups to be associated
          with the            cluster
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