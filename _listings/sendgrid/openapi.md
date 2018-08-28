---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  description: the-sendgrid-web-api-v3-documentation--this-is-the-entirety-of-the-documented-v3-endpoints--we-have-updated-all-the-descriptions-parameters-requests-and-responses--authentication-every-endpoint-requires-authentication-in-the-form-of-an-authorization-header-authorization-bearer-api-key
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
  /user/webhooks/parse/settings:
    get:
      summary: Get User Webhooks Parse Settings
      description: |-
        **This endpoint allows you to retrieve all of your current inbound parse settings.**

        The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
      operationId: user.webhooks.parse.settings.get
      x-api-path-slug: userwebhooksparsesettings-get
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
      - Parse
      - Settings
    post:
      summary: Add User Webhooks Parse Settings
      description: |-
        **This endpoint allows you to create a new inbound parse setting.**

        The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the content, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
      operationId: user.webhooks.parse.settings.post
      x-api-path-slug: userwebhooksparsesettings-post
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
      - Parse
      - Settings
  /user/webhooks/parse/settings/{hostname}:
    delete:
      summary: Delete User Webhooks Parse Settings Hostname
      description: |-
        **This endpoint allows you to delete a specific inbound parse setting.**

        The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
      operationId: user.webhooks.parse.settings.hostname.delete
      x-api-path-slug: userwebhooksparsesettingshostname-delete
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
      - Parse
      - Settings
      - Hostname
    get:
      summary: Get User Webhooks Parse Settings Hostname
      description: |-
        **This endpoint allows you to retrieve a specific inbound parse setting.**

        The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
      operationId: user.webhooks.parse.settings.hostname.get
      x-api-path-slug: userwebhooksparsesettingshostname-get
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
      - Parse
      - Settings
      - Hostname
    patch:
      summary: Patch User Webhooks Parse Settings Hostname
      description: |-
        **This endpoint allows you to update a specific inbound parse setting.**

        The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
      operationId: user.webhooks.parse.settings.hostname.patch
      x-api-path-slug: userwebhooksparsesettingshostname-patch
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
      - Parse
      - Settings
      - Hostname
  /user/webhooks/parse/stats:
    get:
      summary: Get User Webhooks Parse Stats
      description: |-
        **This endpoint allows you to retrieve the statistics for your Parse Webhook useage.**

        SendGrid's Inbound Parse Webhook allows you to parse the contents and attachments of incomming emails. The Parse API can then POST the parsed emails to a URL that you specify. The Inbound Parse Webhook cannot parse messages greater than 20MB in size, including all attachments.

        There are a number of pre-made integrations for the SendGrid Parse Webhook which make processing events easy. You can find these integrations in the [Library Index](https://sendgrid.com/docs/Integrate/libraries.html#-Webhook-Libraries).
      operationId: user.webhooks.parse.stats.get
      x-api-path-slug: userwebhooksparsestats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How you would like the statistics to by grouped
      - in: query
        name: end_date
        description: The end date of the statistics you want to retrieve
      - in: query
        name: limit
        description: The number of statistics to return on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of statistics to skip
      - in: query
        name: start_date
        description: The starting date of the statistics you want to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Webhooks
      - Parse
      - Stats
---