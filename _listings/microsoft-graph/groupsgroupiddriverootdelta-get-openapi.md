---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph API Track Changes For A Drive
  description: Track changes for a Drive This method allows your app to track changes
    to a drive and its children over time.
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