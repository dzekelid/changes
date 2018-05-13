---
swagger: "2.0"
info:
  title: AWS Route 53 API Get Change
  version: 1.0.0
  description: 'Returns the current status of a change batch request. The status is
    one of thefollowing values:                  PENDING indicates that the changes
    in this request have not replicatedto all Amazon Route 53 DNS servers. This is
    the initial status of all change batchrequests.                  INSYNC indicates
    that the changes have replicated to all Amazon Route 53 DNSservers.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/change/Id:
    get:
      summary: Get Change
      description: Returns the current status of a change batch request
      operationId: getchange
      parameters:
      - in: path
        name: Id
        description: The ID of the change batch request
        type: string
      responses:
        200:
          description: OK
      tags:
      - changes
definitions: []
x-collection-name: AWS Route 53
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