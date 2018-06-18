---
swagger: "2.0"
x-collection-name: Tropo
x-complete: 0
info:
  title: Tropo Get Exchanges
  description: Get exchanges.
  version: v1
host: api.tropo.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /exchanges:
    get:
      summary: Get Exchanges
      description: Get exchanges.
      operationId: getExchanges
      x-api-path-slug: exchanges-get
      parameters:
      - in: query
        name: applicationId
      responses:
        200:
          description: OK
      tags:
      - Exchanges
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