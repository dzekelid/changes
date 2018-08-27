{
  "info": {
    "name": "Microsoft Graph API Track Changes For A Drive",
    "_postman_id": "f05bdfd0-0b09-492a-bb29-b381235e960f",
    "description": "Track changes for a Drive This method allows your app to track changes to a drive and its children over time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "track",
      "item": [
        {
          "id": "2802cacf-592e-4df3-9517-fc61cf691fde",
          "name": "TrackChangesForADrive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "drives/:drive-id/root/delta"
              ],
              "variable": [
                {
                  "id": "drive-id",
                  "value": "drive-id",
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
              "id": "44db7902-98f7-4cf6-9748-c7349dc1877b"
            }
          ]
        }
      ]
    }
  ]
}