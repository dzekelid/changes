{
  "info": {
    "name": "Entertainment Express Returns list of unique EpisodeId and Entity changes greater than or equal to date (UTC).",
    "_postman_id": "a0d5fdd4-6a54-4b47-b1d9-70877b0fe932",
    "description": "Lists each episode ID that has changed as well as the entity in the object that changed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Changes",
      "item": [
        {
          "id": "36212f3f-e12b-495d-9940-8c5927d0ccbf",
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
              "id": "83e13796-02f0-4023-b400-62737298bd60"
            }
          ]
        },
        {
          "id": "633f0a2d-574e-4db8-828f-7f6715761c49",
          "name": "GetEpisodeChangeHistoryWithEntity",
          "request": {
            "url": "http://ee.iva-api.com/Changes/Episodes/HistoryWithEntity/?Date=%7B%7D&Skip=%7B%7D&Take=%7B%7D",
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
            "description": "Lists each episode ID that has changed as well as the entity in the object that changed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5f322c2-96ab-49bc-b7d4-a56014cb0e45"
            }
          ]
        }
      ]
    }
  ]
}