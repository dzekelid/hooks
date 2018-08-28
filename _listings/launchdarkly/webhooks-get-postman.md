{
  "info": {
    "name": "Launch Darkly Fetch a list of all webhooks",
    "_postman_id": "99a36650-98da-498c-b794-bd5b0c895fd6",
    "description": "Fetch a list of all webhooks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "34816544-4d19-4384-beec-86d619cfe067",
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
              "id": "f2e3ec38-2521-4391-9363-3c559a0d4ed2"
            }
          ]
        }
      ]
    }
  ]
}