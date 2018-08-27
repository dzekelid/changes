{
  "info": {
    "name": "Entertainment Express Returns list of unique EpisodeId changes greater than or equal to date (UTC)",
    "_postman_id": "4baa0963-a72d-4ee1-ac7a-c476b040e8d1",
    "description": "For each updated episode ID, pull the full episode data for that ID and update.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Changes",
      "item": [
        {
          "id": "92789cf5-9124-459f-bed0-d9328107d744",
          "name": "GetEpisodeChangeHistory",
          "request": {
            "url": "http://ee.iva-api.com/Changes/Episodes/History/?Date=%7B%7D&Skip=%7B%7D&Take=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "For each updated episode ID, pull the full episode data for that ID and update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cedd5a1-d283-429d-ac8c-9196224f2f45"
            }
          ]
        }
      ]
    }
  ]
}