{
  "info": {
    "name": "Eventbrite Get Webhooks",
    "_postman_id": "6e200e48-7c56-4e1a-b9a4-a87058414b02",
    "description": "Returns the list of webhook objects that belong to the authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "2be2a1b2-7de2-4eb2-8935-315a31240594",
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
              "id": "e9377219-6e04-4b5e-af7c-de01320456cd"
            }
          ]
        },
        {
          "id": "c29072b8-bf39-4d22-8258-0060518ac38a",
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
              "id": "faff83c1-f062-4aa8-b7f5-c400a0e96607"
            }
          ]
        },
        {
          "id": "c1dc8a74-e2f6-49f8-96cd-262cd9f76dc9",
          "name": "getWebhooks1",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/webhooks/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of webhook objects that belong to the authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad3bc7e4-7da8-40db-b5e9-3cb4a3797590"
            }
          ]
        }
      ]
    }
  ]
}