{
  "info": {
    "name": "Launch Darkly Delete a webhook by ID",
    "_postman_id": "14475905-a929-4e74-b39b-af5e180b78be",
    "description": "Delete a webhook by id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "22deef8d-22d9-4bdd-b629-49d09565e5ed",
          "name": "getWebhooks",
          "request": {
            "url": "http://app.launchdarkly.com/api/v2/webhooks",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch a list of all webhooks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c511f98-5bc3-4edd-b8ac-82fa8ebd057b"
            }
          ]
        },
        {
          "id": "07784e03-d676-4289-8cee-4d03c349b6f9",
          "name": "postWebhook",
          "request": {
            "url": "http://app.launchdarkly.com/api/v2/webhooks?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a webhook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ebc1d82-89e0-4b22-b592-63ceb4a673ef"
            }
          ]
        },
        {
          "id": "d5d77805-2656-4d45-8cc9-dc1877d5b125",
          "name": "deleteWebhook",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "webhooks/:resourceId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceId",
                  "value": "resourceId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a webhook by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e718ba9-3115-4497-ac14-dbac98ae9b4f"
            }
          ]
        }
      ]
    }
  ]
}