---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Add User Webhooks Event Test
  description: "**This endpoint allows you to test your event webhook by sending a
    fake event notification post to the provided URL.**\n\nSendGrid\u2019s Event Webhook
    will notify a URL of your choice via HTTP POST with information about events that
    occur as SendGrid processes your email.\n\nCommon uses of this data are to remove
    unsubscribes, react to spam reports, determine unengaged recipients, identify
    bounced email addresses, or create advanced analytics of your email program."
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/webhooks/event/settings:
    get:
      summary: Get User Webhooks Event Settings
      description: "**This endpoint allows you to retrieve your current event webhook
        settings.**\n\nIf an event type is marked as `true`, then the event webhook
        will include information about that event.\n\nSendGrid\u2019s Event Webhook
        will notify a URL of your choice via HTTP POST with information about events
        that occur as SendGrid processes your email.\n\nCommon uses of this data are
        to remove unsubscribes, react to spam reports, determine unengaged recipients,
        identify bounced email addresses, or create advanced analytics of your email
        program."
      operationId: user.webhooks.event.settings.get
      x-api-path-slug: userwebhookseventsettings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Webhooks
      - Event
      - Settings
    patch:
      summary: Patch User Webhooks Event Settings
      description: "**This endpoint allows you to update your current event webhook
        settings.**\n\nIf an event type is marked as `true`, then the event webhook
        will include information about that event.\n\nSendGrid\u2019s Event Webhook
        will notify a URL of your choice via HTTP POST with information about events
        that occur as SendGrid processes your email.\n\nCommon uses of this data are
        to remove unsubscribes, react to spam reports, determine unengaged recipients,
        identify bounced email addresses, or create advanced analytics of your email
        program."
      operationId: user.webhooks.event.settings.patch
      x-api-path-slug: userwebhookseventsettings-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Webhooks
      - Event
      - Settings
  /user/webhooks/event/test:
    post:
      summary: Add User Webhooks Event Test
      description: "**This endpoint allows you to test your event webhook by sending
        a fake event notification post to the provided URL.**\n\nSendGrid\u2019s Event
        Webhook will notify a URL of your choice via HTTP POST with information about
        events that occur as SendGrid processes your email.\n\nCommon uses of this
        data are to remove unsubscribes, react to spam reports, determine unengaged
        recipients, identify bounced email addresses, or create advanced analytics
        of your email program."
      operationId: user.webhooks.event.test.post
      x-api-path-slug: userwebhookseventtest-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Webhooks
      - Event
      - Test
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