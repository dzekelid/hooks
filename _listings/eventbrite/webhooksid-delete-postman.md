{
  "info": {
    "name": "Eventbrite Delete Webhooks",
    "_postman_id": "24e6f9f9-83fa-4841-90ee-7705b2d45a21",
    "description": "Deletes the specified webhook object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "3e67a8e4-a65d-4831-8e9c-47881f267c92",
          "name": "getWebhooks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "webhooks/:id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a webhook for the specified webhook as webhook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26b43eaa-ccf8-4bb4-a57c-7d1e601222b9"
            }
          ]
        },
        {
          "id": "eb46464d-1655-4b79-95fc-b2f516aeb5aa",
          "name": "deleteWebhooks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "webhooks/:id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified webhook object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aad3ad65-34ee-4ea8-9c81-444ecbc96387"
            }
          ]
        }
      ]
    }
  ]
}