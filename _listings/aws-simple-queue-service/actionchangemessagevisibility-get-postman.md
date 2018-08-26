{
  "info": {
    "name": "AWS Simple Queue Service API Change Message Visibility",
    "_postman_id": "541a679b-89c0-4cd6-a867-9287a7038a53",
    "description": "Changes the visibility timeout of a specified message in a queue to a new value.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "bba657db-1b1c-45de-a644-25ef7e6ccb04",
          "name": "addPermission",
          "request": {
            "url": "http://example.com/api/?Action=AddPermission?ActionName.N=ActionName.N&AWSAccountId.N=AWSAccountId.N&Label=Label&QueueUrl=QueueUrl",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a permission to a queue for a specific."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7222f9b-f8fe-411a-9bff-0ff4faae596b"
            }
          ]
        }
      ]
    },
    {
      "name": "Message Visibility",
      "item": [
        {
          "id": "22e5b582-d03d-4ea7-b6b0-0eee2850f61d",
          "name": "changeMessageVisibility",
          "request": {
            "url": "http://example.com/api/?Action=ChangeMessageVisibility?QueueUrl=QueueUrl&ReceiptHandle=ReceiptHandle&VisibilityTimeout=VisibilityTimeout",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Changes the visibility timeout of a specified message in a queue to a new value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63a60b2b-57bb-4413-8353-2b9d95cfeb9c"
            }
          ]
        }
      ]
    }
  ]
}