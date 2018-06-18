---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/drive/root/delta:
    get:
      summary: Track Changes For A Drive
      description: Track changes for a Drive This method allows your app to track
        changes to a drive and its children over time.
      operationId: TrackChangesForADrive
      x-api-path-slug: medriverootdelta-get
      responses:
        200:
          description: OK
      tags:
      - Track
      - Changes
      - Drive
  /drives/{drive-id}/root/delta:
    get:
      summary: Track Changes For A Drive
      description: Track changes for a Drive This method allows your app to track
        changes to a drive and its children over time.
      operationId: TrackChangesForADrive
      x-api-path-slug: drivesdriveidrootdelta-get
      parameters:
      - in: path
        name: drive-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Track
      - Changes
      - Drive
  /groups/{group-id}/drive/root/delta:
    get:
      summary: Track Changes For A Drive
      description: Track changes for a Drive This method allows your app to track
        changes to a drive and its children over time.
      operationId: TrackChangesForADrive
      x-api-path-slug: groupsgroupiddriverootdelta-get
      parameters:
      - in: path
        name: group-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Track
      - Changes
      - Drive
---