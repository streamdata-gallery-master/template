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
  /?Action=CreateCluster&k=1:
    get:
      summary: ' Create Cluster '
      description: Creates a new cluster
      operationId: createCluster
      parameters:
      - in: query
        name: AdditionalInfo
        description: Reserved
        type: string
      - in: query
        name: AllowVersionUpgrade
        description: If true, major version upgrades can be applied during the maintenance            window
          to the Amazon Redshift engine that is running on the cluster
        type: string
      - in: query
        name: AutomatedSnapshotRetentionPeriod
        description: The number of days that automated snapshots are retained
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone (AZ) in which you want Amazon Redshift
          to provision the            cluster
        type: string
      - in: query
        name: ClusterIdentifier
        description: A unique identifier for the cluster
        type: string
      - in: query
        name: ClusterParameterGroupName
        description: The name of the parameter group to be associated with this cluster
        type: string
      - in: query
        name: ClusterSecurityGroups.ClusterSecurityGroupName.N
        description: A list of security groups to be associated with this cluster
        type: string
      - in: query
        name: ClusterSubnetGroupName
        description: The name of a cluster subnet group to be associated with this
          cluster
        type: string
      - in: query
        name: ClusterType
        description: The type of the cluster
        type: string
      - in: query
        name: ClusterVersion
        description: The version of the Amazon Redshift engine software that you want
          to deploy on the            cluster
        type: string
      - in: query
        name: DBName
        description: The name of the first database to be created when the cluster
          is created
        type: string
      - in: query
        name: ElasticIp
        description: The Elastic IP (EIP) address for the cluster
        type: string
      - in: query
        name: Encrypted
        description: If true, the data in the cluster is encrypted at rest
        type: string
      - in: query
        name: EnhancedVpcRouting
        description: An option that specifies whether to create the cluster with enhanced
          VPC routing            enabled
        type: string
      - in: query
        name: HsmClientCertificateIdentifier
        description: Specifies the name of the HSM client certificate the Amazon Redshift
          cluster uses to           retrieve the data encryption keys stored in an
          HSM
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: Specifies the name of the HSM configuration that contains the
          information the            Amazon Redshift cluster can use to retrieve and
          store keys in an HSM
        type: string
      - in: query
        name: IamRoles.IamRoleArn.N
        description: A list of AWS Identity and Access Management (IAM) roles that
          can be used by the            cluster to access other AWS services
        type: string
      - in: query
        name: KmsKeyId
        description: The AWS Key Management Service (KMS) key ID of the encryption
          key that you want to            use to encrypt data in the cluster
        type: string
      - in: query
        name: MasterUsername
        description: The user name associated with the master user account for the
          cluster that is being            created
        type: string
      - in: query
        name: MasterUserPassword
        description: The password associated with the master user account for the
          cluster that is being            created
        type: string
      - in: query
        name: NodeType
        description: The node type to be provisioned for the cluster
        type: string
      - in: query
        name: NumberOfNodes
        description: The number of compute nodes in the cluster
        type: string
      - in: query
        name: Port
        description: The port number on which the cluster accepts incoming connections
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which automated cluster
          maintenance can            occur
        type: string
      - in: query
        name: PubliclyAccessible
        description: If true, the cluster can be accessed from a public network
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of Virtual Private Cloud (VPC) security groups to be associated
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