---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Changes the owning team of an event
  version: 1.0.0
  description: Changes the owning team of an event.
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
  /api/event/{id}/setowningteam:
    put:
      summary: Changes the owning team of an event
      description: Changes the owning team of an event.
      operationId: Event_SetOwningTeamByidByteamId
      x-api-path-slug: apieventidsetowningteam-put
      parameters:
      - in: path
        name: id
        description: Event Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: Team Id for new owning team
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Owning
      - Team
      - Of
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