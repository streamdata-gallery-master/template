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
  /?Action=GetJobManifest&k=1:
    get:
      summary: ' Get Job Manifest '
      description: |-
        Returns a link to an Amazon S3 presigned URL for the manifest file associated with the
              specified JobId value
      operationId: getJobManifest
      parameters:
      - in: query
        name: JobId
        description: The ID for a job that you want to get the manifest file for,
          for example        JID123e4567-e89b-12d3-a456-426655440000
        type: string
      responses:
        200:
          description: OK
      tags:
      - job manifest
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