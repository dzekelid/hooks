{
  "info": {
    "name": "Launch Darkly Create a webhook",
    "_postman_id": "14108315-ab5c-46d8-a36f-e802d8593a6c",
    "description": "Create a webhook.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "e7d5466a-f9d3-4484-852d-93b873af39af",
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
              "id": "1c7e7acc-8876-4704-af86-e708a1877ee8"
            }
          ]
        },
        {
          "id": "cc30d0aa-7c24-403a-8be8-37c9a4b472b6",
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
              "id": "2ffe5a22-c370-4d43-adb7-5ad06978e9a4"
            }
          ]
        }
      ]
    }
  ]
}