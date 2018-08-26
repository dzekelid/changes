---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/merge_request/{merge_request_id}/changes:
    get:
      summary: Get Projects Merge Request Merge Request Changes
      description: Get projects merge request merge request changes.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdChanges
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idchanges-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Changes
  /v3/projects/{id}/merge_requests/{merge_request_id}/changes:
    get:
      summary: Get Projects Merge Requests Merge Request Changes
      description: Get projects merge requests merge request changes.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdChanges
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idchanges-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Changes
---