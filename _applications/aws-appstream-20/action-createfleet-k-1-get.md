---
swagger: "2.0"
info:
  title: AWS AppStream 2.0 API
  description: Amazon AppStream 2.0 is a fully managed, secure application streaming
    service that allows you to stream desktop applications from AWS to any device
    running a web browser, without rewriting them. Amazon AppStream 2.0 provides users
    instant-on access to the applications they need, and a responsive, fluid user
    experience on the device of their choice.
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateFleet&k=1:
    get:
      summary: Create Fleet
      description: Creates a new fleet
      operationId: CreateFleet
      parameters:
      - in: query
        name: ComputeCapacity
        description: The parameters for the capacity allocated to the fleet
        type: string
      - in: query
        name: Description
        description: The description of the fleet
        type: string
      - in: query
        name: DisconnectTimeoutInSeconds
        description: The time after disconnection when a session is considered to
          have ended
        type: string
      - in: query
        name: DisplayName
        description: The display name of the fleet
        type: string
      - in: query
        name: ImageName
        description: Unique name of the image used by the fleet
        type: string
      - in: query
        name: InstanceType
        description: The instance type of compute resources for the fleet
        type: string
      - in: query
        name: MaxUserDurationInSeconds
        description: The maximum time up to which a streaming session can run
        type: string
      - in: query
        name: Name
        description: A unique identifier for the fleet
        type: string
      - in: query
        name: VpcConfig
        description: The VPC configuration for the fleet
        type: string
      responses:
        200:
          description: OK
      tags:
      - fleet
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