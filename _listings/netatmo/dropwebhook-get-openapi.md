---
swagger: "2.0"
x-collection-name: Netatmo
x-complete: 0
info:
  title: Netatmo Get Dropwebhook
  description: Dissociates a webhook from a user.
  termsOfService: https://dev.netatmo.com/dev/resources/legal/introduction
  contact:
    name: Netatmo
    email: contact-api@netatmo.com
  version: 1.1.1
host: api.netatmo.net
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /addwebhook:
    get:
      summary: Get Addwebhook
      description: Links a callback url to a user.
      operationId: addwebhook
      x-api-path-slug: addwebhook-get
      parameters:
      - in: query
        name: app_type
        description: Webhooks are only available for Welcome, enter app_camera
      - in: query
        name: url
        description: Your webhook callback url
      responses:
        200:
          description: OK
      tags:
      - Web Hooks
  /dropwebhook:
    get:
      summary: Get Dropwebhook
      description: Dissociates a webhook from a user.
      operationId: dropwebhook
      x-api-path-slug: dropwebhook-get
      parameters:
      - in: query
        name: app_type
        description: For Welcome, use app_camera
      responses:
        200:
          description: OK
      tags:
      - Web Hooks
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---