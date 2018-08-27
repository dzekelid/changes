swagger: "2.0"
x-collection-name: Getty Images
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
  version: 1.0.0
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/asset-changes/change-sets:
    put:
      summary: Get Asset Change Notifications
      description: "# Asset Changes\r\n\r\nGet notifications about new, updated or
        deleted assets.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a
        [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n    \r\nPartner
        channels that have not been checked within the last 120 days will be removed
        and that partner will no longer be able \r\nto get change notifications from
        that channel.\r\nPartners who would like to start using the Asset Changes
        API again after a period of dormancy should contact their sales\r\nrepresentative
        to be set up again."
      operationId: AssetChanges_PutAssetChanges
      x-api-path-slug: v3assetchangeschangesets-put
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: batch_size
        description: Specifies the number of assets to return
      - in: query
        name: channel_id
        description: Specifies the id of the channel for the asset data
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes
  /v3/asset-changes/change-sets/{change-set-id}:
    delete:
      summary: Get Asset Change Notification
      description: "# Delete Asset Changes\r\n\r\nConfirm asset changes acknowledges
        receipt of asset changes (from the PUT asset changes endpoint).\r\n\r\n##
        \ Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: AssetChanges_DeleteAssetChanges
      x-api-path-slug: v3assetchangeschangesetschangesetid-delete
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: change-set-id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes
  /v3/asset-changes/channels:
    get:
      summary: Get Asset Change Channels
      description: "# Get Partner Channels\r\n\r\nRetrieves the channel data for the
        partner. This data can be used to populate the channel_id parameter in the
        Put Asset Changes query.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key
        and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\nOnly channels
        that have been queried in the last 120 days will be included in the list of
        channels.\r\nPartners who have a channel that has been removed should contact
        their sales representative to be set up again."
      operationId: AssetChanges_GetPartnerChannel
      x-api-path-slug: v3assetchangeschannels-get
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes