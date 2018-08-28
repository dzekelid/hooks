{
  "info": {
    "name": "Eventbrite Get Webhooks",
    "_postman_id": "dfd087f0-94c8-4f82-8bfe-37ac1e198bb2",
    "description": "Returns a webhook for the specified webhook as webhook.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "b85836ae-63a3-49a8-968e-8b4ffdcdc8cc",
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
              "id": "a5bec482-c4b3-4ffb-a521-1035e54dbee0"
            }
          ]
        }
      ]
    }
  ]
}