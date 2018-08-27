{
  "info": {
    "name": "Microsoft Graph API Track Changes For A Drive",
    "_postman_id": "529830b6-996f-4870-8908-9149885fb387",
    "description": "Track changes for a Drive This method allows your app to track changes to a drive and its children over time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "track",
      "item": [
        {
          "id": "e2b83d7e-aeeb-42e4-a47b-0d091d1d62b7",
          "name": "TrackChangesForADrive",
          "request": {
            "url": "http://graph.microsoft.com/me/drive/root/delta",
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
              "id": "4316a48e-0fd5-4416-b9f7-3b604b8ebc6c"
            }
          ]
        }
      ]
    }
  ]
}