{
  "info": {
    "name": "AWS Simple Queue Service API Change Message Visibility Batch",
    "_postman_id": "411873dc-3300-4651-907c-3becb0046945",
    "description": "Changes the visibility timeout of multiple messages.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "eca7885f-7766-4037-b21e-efe363b77d41",
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
              "id": "af78adf0-f895-4b0d-8134-6de476cc8bd9"
            }
          ]
        }
      ]
    },
    {
      "name": "Message Visibility",
      "item": [
        {
          "id": "72d16fe5-cf75-45c7-9b86-cc030c32199b",
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
              "id": "4de2b3d8-ec1a-4602-86a0-03314d34992f"
            }
          ]
        },
        {
          "id": "95f8d35e-37d5-40a5-bf48-d55d128cac52",
          "name": "changeMessageVisibilityBatch",
          "request": {
            "url": "http://example.com/api/?Action=ChangeMessageVisibilityBatch?ChangeMessageVisibilityBatchRequestEntry.N=ChangeMessageVisibilityBatchRequestEntry.N&QueueUrl=QueueUrl",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Changes the visibility timeout of multiple messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09a53d64-7a7b-4173-9d5d-8d91cca75a5c"
            }
          ]
        }
      ]
    }
  ]
}