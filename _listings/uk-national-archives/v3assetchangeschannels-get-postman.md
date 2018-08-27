{
  "info": {
    "name": "Getty Images Search API Get Asset Changes Channels",
    "_postman_id": "f873953e-fa85-450d-860e-960c0754943a",
    "description": "Retrieves the channel data for the partner. this data can be used to populate the channel_id parameter in the put asset changes query..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Asset",
      "item": [
        {
          "id": "7efa2d85-8847-40a7-883e-73b45fae2007",
          "name": "putV3AssetChangesChangeSets",
          "request": {
            "url": "http://api.gettyimages.com/v3/asset-changes/change-sets?batch_size=%7B%7D&channel_id=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "Accept-Language",
                "value": "{}",
                "description": "Accept-Language parameter optional",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Authorization token required",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Generates asset changes.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cdc819e-7c1b-4b69-8f42-dae56dd679e1"
            }
          ]
        },
        {
          "id": "5fa2cba3-3f4b-484b-af11-40a774954616",
          "name": "deleteV3AssetChangesChangeSetsChangeSet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/asset-changes/change-sets/:change-set-id"
              ],
              "variable": [
                {
                  "id": "change-set-id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept-Language",
                "value": "{}",
                "description": "Accept-Language parameter optional",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Authorization token required",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Confirm asset changes acknowledges receipt of asset changes.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed7daebb-93fa-4514-a6a5-084784edf502"
            }
          ]
        },
        {
          "id": "6402e85b-928b-44bf-858d-cad54d4531a4",
          "name": "getV3AssetChangesChannels",
          "request": {
            "url": "http://api.gettyimages.com/v3/asset-changes/channels",
            "method": "GET",
            "header": [
              {
                "key": "Accept-Language",
                "value": "{}",
                "description": "Accept-Language parameter optional",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Authorization token required",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the channel data for the partner. this data can be used to populate the channel_id parameter in the put asset changes query.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "930cb68d-9812-4654-9f4e-c2e749766198"
            }
          ]
        }
      ]
    }
  ]
}