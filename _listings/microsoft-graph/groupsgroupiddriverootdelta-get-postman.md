{
  "info": {
    "name": "Microsoft Graph API Track Changes For A Drive",
    "_postman_id": "b04521fb-19c0-43b0-a473-1e2720131536",
    "description": "Track changes for a Drive This method allows your app to track changes to a drive and its children over time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "track",
      "item": [
        {
          "id": "6ef8f101-fd13-403a-8492-31537876a3ec",
          "name": "TrackChangesForADrive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:group-id/drive/root/delta"
              ],
              "variable": [
                {
                  "id": "group-id",
                  "value": "group-id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Track changes for a Drive This method allows your app to track changes to a drive and its children over time"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "1beb8888-ec61-453f-bc2f-e2defb81f913"
            }
          ]
        }
      ]
    }
  ]
}