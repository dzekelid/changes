---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 0
info:
  title: Akamai API Delete an Enrollment
  description: Delete an Enrollment
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cps/v2/enrollments/{enrollmentId}:
    put:
      summary: Update an Enrollment
      description: Update an Enrollment
      operationId: cpsv2enrollmentsenrollmentiddeploynotbeforedeploynotafterallowcancelpendingchanges
      x-api-path-slug: cpsv2enrollmentsenrollmentid-put
      parameters:
      - in: query
        name: allow-cancel-pending-changes
        description: When enabled, allows this update to cancel and replace in-process
          changes
        type: string
      - in: query
        name: deploy-not-after
        description: The latest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: query
        name: deploy-not-before
        description: The earliest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: query
        name: enrollmentId
        description: Integer identifier for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
      - Deploy
      - Not
      - Before
      - deploy
      - Not
      - After
      - allow
      - Cancel
      - Pending
      - Changes
    delete:
      summary: Delete an Enrollment
      description: Delete an Enrollment
      operationId: cpsv2enrollmentsenrollmentiddeploynotbeforedeploynotafterallowcancelpendingchanges
      x-api-path-slug: cpsv2enrollmentsenrollmentid-delete
      parameters:
      - in: query
        name: allow-cancel-pending-changes
        description: When enabled, allows this update to cancel and replace in-process
          changes
        type: string
      - in: query
        name: deploy-not-after
        description: The latest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: query
        name: deploy-not-before
        description: The earliest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: query
        name: enrollmentId
        description: Integer identifier for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
      - Deploy
      - Not
      - Before
      - deploy
      - Not
      - After
      - allow
      - Cancel
      - Pending
      - Changes
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