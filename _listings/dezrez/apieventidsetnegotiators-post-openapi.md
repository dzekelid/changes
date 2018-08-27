---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Changes the negotiators for an event
  version: 1.0.0
  description: Changes the negotiators for an event.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/event/{id}/setnegotiators:
    post:
      summary: Changes the negotiators for an event
      description: Changes the negotiators for an event.
      operationId: Event_SetNegotiatorsByidBycommandDataContract
      x-api-path-slug: apieventidsetnegotiators-post
      parameters:
      - in: body
        name: commandDataContract
        description: Command Data Contract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Event Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Negotiatorsan
      - Event
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