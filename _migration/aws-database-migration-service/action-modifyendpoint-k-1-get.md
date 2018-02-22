---
swagger: "2.0"
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyEndpoint&k=1:
    get:
      summary: ' Modify Endpoint '
      description: Modifies the specified endpoint
      operationId: modifyEndpoint
      parameters:
      - in: query
        name: CertificateArn
        description: The Amazon Resource Name (ARN) of the certificate used for SSL
          connection
        type: string
      - in: query
        name: DatabaseName
        description: The name of the endpoint database
        type: string
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: EndpointIdentifier
        description: The database endpoint identifier
        type: string
      - in: query
        name: EndpointType
        description: The type of endpoint
        type: string
      - in: query
        name: EngineName
        description: The type of engine for the endpoint
        type: string
      - in: query
        name: ExtraConnectionAttributes
        description: Additional attributes associated with the connection
        type: string
      - in: query
        name: Password
        description: The password to be used to login to the endpoint database
        type: string
      - in: query
        name: Port
        description: The port used by the endpoint database
        type: string
      - in: query
        name: ServerName
        description: The name of the server where the endpoint database resides
        type: string
      - in: query
        name: SslMode
        description: The SSL mode to be used
        type: string
      - in: query
        name: Username
        description: The user name to be used to login to the endpoint database
        type: string
      responses:
        200:
          description: OK
      tags:
      - endpoints
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