---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Update Signing Certificate
  version: 1.0.0
  description: |-
    Changes the status of the specified user signing certificate from active to disabled,
          or vice versa.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ChangePassword:
    get:
      summary: Change Password
      description: Changes the password of the IAM user who is calling this action.
      operationId: changePassword
      x-api-path-slug: actionchangepassword-get
      parameters:
      - in: query
        name: NewPassword
        description: The new password
        type: string
      - in: query
        name: OldPassword
        description: The IAM users current password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Passwords
  /?Action=UpdateAccessKey:
    get:
      summary: Update Access Key
      description: Changes the status of the specified access key from Active to Inactive,
        or vice versa.
      operationId: updateAccessKey
      x-api-path-slug: actionupdateaccesskey-get
      parameters:
      - in: query
        name: AccessKeyId
        description: The access key ID of the secret access key you want to update
        type: string
      - in: query
        name: Status
        description: The status you want to assign to the secret access key
        type: string
      - in: query
        name: UserName
        description: The name of the user whose key you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=UpdateLoginProfile:
    get:
      summary: Update Login Profile
      description: Changes the password for the specified IAM user.
      operationId: updateLoginProfile
      x-api-path-slug: actionupdateloginprofile-get
      parameters:
      - in: query
        name: Password
        description: The new password for the specified IAM user
        type: string
      - in: query
        name: PasswordResetRequired
        description: Allows this new password to be used only once by requiring the
          specified IAM user to      set a new password on next sign-in
        type: string
      - in: query
        name: UserName
        description: The name of the user whose password you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
  /?Action=UpdateSigningCertificate:
    get:
      summary: Update Signing Certificate
      description: |-
        Changes the status of the specified user signing certificate from active to disabled,
              or vice versa.
      operationId: updateSigningCertificate
      x-api-path-slug: actionupdatesigningcertificate-get
      parameters:
      - in: query
        name: CertificateId
        description: The ID of the signing certificate you want to update
        type: string
      - in: query
        name: Status
        description: The status you want to assign to the certificate
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user the signing certificate belongs to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signing Certificates
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