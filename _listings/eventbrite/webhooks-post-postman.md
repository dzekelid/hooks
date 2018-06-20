{
  "info": {
    "name": "Eventbrite Add Webhooks",
    "_postman_id": "88cf8972-b477-4d1e-8a39-870f1a0dcc1e",
    "description": "Creates a webhook for the authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "a6b3298e-576e-4401-8088-eda9ba14bbec",
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
              "id": "ae8dfa71-94b5-4ab6-9811-e877ae5a852d"
            }
          ]
        },
        {
          "id": "291b0510-b84b-488d-b7dc-9522578025f2",
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
              "id": "679eef2d-859e-4fbb-9280-56fc5507904e"
            }
          ]
        },
        {
          "id": "9a51bcf3-835d-4534-a20c-352ee5abf448",
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
              "id": "a5bc281d-aaf7-4b56-964d-cf52b7bcefd9"
            }
          ]
        },
        {
          "id": "4aec9765-de5f-428d-9a25-17047f71bc95",
          "name": "postWebhooks",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/webhooks/?actions=%7B%7D&endpoint_url=%7B%7D&event_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a webhook for the authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99a2937d-04c1-44dc-a60b-af2cd4656b72"
            }
          ]
        }
      ]
    }
  ]
}