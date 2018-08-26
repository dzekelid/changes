---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
---