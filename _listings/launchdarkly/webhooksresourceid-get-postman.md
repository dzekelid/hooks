{
  "info": {
    "name": "Launch Darkly Get a webhook by ID",
    "_postman_id": "bbb4b940-6727-45fe-8a72-9928bc2a08ea",
    "description": "Get a webhook by id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "c0df29d8-f784-4688-85c9-17c64f81e90c",
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
              "id": "4f844167-a344-4ee8-b919-4792a5617aaa"
            }
          ]
        },
        {
          "id": "b044f228-e1e2-41c6-a415-882b97ffd1d1",
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
              "id": "2fd094dd-630f-406f-9bfd-84193c121e63"
            }
          ]
        },
        {
          "id": "dfbe62d4-95c9-4d0c-bd15-4548429ac093",
          "name": "getWebhook",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a webhook by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cca84a7d-388c-4035-9628-b75dfc5527af"
            }
          ]
        },
        {
          "id": "021f005c-f833-401c-8357-270b52f91a78",
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
              "id": "7e504ce3-8e16-4990-a85c-e237477fee46"
            }
          ]
        }
      ]
    }
  ]
}