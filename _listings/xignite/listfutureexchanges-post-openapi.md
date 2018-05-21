---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Real Time Futures List Future Exchanges
  description: Returns a list of future exchanges
  version: 1.0.0
host: globalrealtimefutures.xignite.com
basePath: xGlobalRealTimeFutures.json/XigniteGlobalRealTimeFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListFutureExchanges:
    post:
      summary: List Future Exchanges
      description: Returns a list of future exchanges
      operationId: ListFutureExchanges
      x-api-path-slug: listfutureexchanges-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Future
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