{
  "info": {
    "name": "Netatmo Get Dropwebhook",
    "_postman_id": "9da3a356-348a-452e-977c-7b6e4089f6d9",
    "description": "Dissociates a webhook from a user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web Hooks",
      "item": [
        {
          "id": "3d0e3919-edc6-429b-b549-68071f52d6a2",
          "name": "addwebhook",
          "request": {
            "url": "http://api.netatmo.net/api/addwebhook?app_type=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Links a callback url to a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abe2716a-4461-4f2b-999e-e94141886012"
            }
          ]
        },
        {
          "id": "7828c728-3226-448e-9616-b9edd20efb7d",
          "name": "dropwebhook",
          "request": {
            "url": "http://api.netatmo.net/api/dropwebhook?app_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Dissociates a webhook from a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76b1530b-dd80-4c7b-8b50-33abfc460781"
            }
          ]
        }
      ]
    }
  ]
}