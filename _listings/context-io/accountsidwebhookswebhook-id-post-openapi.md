---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Post Accounts Webhooks Webhook
  description: |-
    Changes properties of a given WebHook. The only property of a WebHook that can be changed is it's active property. If you want to change the filters or callback urls, delete it and create a new one.
    Changing the active property can be useful in two cases:
    - Pause/resume WebHooks: If your application needs up-to-date information when users are logged in the best option is to keep a WebHook with no filters on that account that will be resumed (setting active to 1) when the user logs in and paused (setting active to 0) when the user logs out of your app.
    - Acting upon a failure notification: If a WebHook fails, your failure_notif_url is called (see creating a WebHook) an its active property becomes 0. Set the active property back to 1 to get it working again.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/files/{fileId}/changes:
    get:
      summary: Get Accounts Files Fileid Changes
      description: Lists files that can be compared with a given file.
      operationId: listComparableAccountFiles_
      x-api-path-slug: accountsidfilesfileidchanges-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Changes
  /accounts/{id}/webhooks/{webhook_id}:
    post:
      summary: Post Accounts Webhooks Webhook
      description: |-
        Changes properties of a given WebHook. The only property of a WebHook that can be changed is it's active property. If you want to change the filters or callback urls, delete it and create a new one.
        Changing the active property can be useful in two cases:
        - Pause/resume WebHooks: If your application needs up-to-date information when users are logged in the best option is to keep a WebHook with no filters on that account that will be resumed (setting active to 1) when the user logs in and paused (setting active to 0) when the user logs out of your app.
        - Acting upon a failure notification: If a WebHook fails, your failure_notif_url is called (see creating a WebHook) an its active property becomes 0. Set the active property back to 1 to get it working again.
      operationId: modifyAccountWebhook_
      x-api-path-slug: accountsidwebhookswebhook-id-post
      parameters:
      - in: query
        name: active
        description: The active property of a WebHook allows you to pause (set to
          0) or resume (set to 1) it
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: webhook_id
        description: Unique id of the webhook instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
      - Webhook
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