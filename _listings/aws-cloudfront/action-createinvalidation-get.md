---
swagger: "2.0"
info:
  title: AWS CloudFront API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateInvalidation:
    get:
      summary: ' Create Invalidation '
      description: Create a new invalidation
      operationId: createInvalidation
      parameters:
      - in: query
        name: DistributionId
        description: The distribution's id
        type: string
      - in: query
        name: DryRun
        description: "Checks whether you have the required permissions for the action,
          without actually making the request, \t\t    and provides an error response"
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - invalidation
definitions: []
x-collection-name: AWS CloudFront
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