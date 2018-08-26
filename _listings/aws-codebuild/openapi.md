---
swagger: "2.0"
x-collection-name: AWS CodeBuild
x-complete: 1
info:
  title: AWS CodeBuild API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateProject:
    get:
      summary: Update Project
      description: Changes the settings of an existing build project.
      operationId: updateProject
      x-api-path-slug: actionupdateproject-get
      parameters:
      - in: query
        name: artifacts
        description: Information to be changed about the build projects build output
          artifacts
        type: string
      - in: query
        name: description
        description: A new or replacement description of the build project
        type: string
      - in: query
        name: encryptionKey
        description: The replacement AWS Key Management Service (AWS KMS) customer
          master key (CMK) to be used for encrypting the build projects build output
          artifacts
        type: string
      - in: query
        name: environment
        description: Information to be changed about the build projects build environment
        type: string
      - in: query
        name: name
        description: The name of the existing build project to change settings
        type: string
      - in: query
        name: serviceRole
        description: The replacement Amazon Resource Name (ARN) of the AWS Identity
          and Access Management (IAM) role that enables AWS CodeBuild to interact
          with dependent AWS services on behalf of the AWS account
        type: string
      - in: query
        name: source
        description: Information to be changed about the build projects build input
          source code
        type: string
      - in: query
        name: tags
        description: The replacement set of tags for this build project
        type: string
      - in: query
        name: timeoutInMinutes
        description: The replacement value in minutes, from 5 to 480 (8 hours), for
          AWS CodeBuild to wait to timeout any related build that did not get marked
          as completed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Projects
---