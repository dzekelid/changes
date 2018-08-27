swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
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
      description: Changes the password for a specified user in a user pool.
      operationId: changePassword
      x-api-path-slug: actionchangepassword-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token in the change password request
        type: string
      - in: query
        name: PreviousPassword
        description: The old password in the change password request
        type: string
      - in: query
        name: ProposedPassword
        description: The new password in the change password request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Password