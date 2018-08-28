---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find webhook resources
  description: 'Searches for webhook resources. Available resources include ''CccCampaign'':
    [''started'', ''stopped'', ''finished''], ''CallBroadcast'': [''started'', ''stopped'',
    ''finished''], ''TextBroadcast'': [''started'', ''stopped'', ''finished''], ''OutboundCall'':
    [''finished''], ''InboundCall'': [''finished''], ''OutboundText'': [''finished''],
    ''InboundText'': [''finished''], ''ContactList'': [''validationFinished'', ''validationFailed'']'
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /webhooks:
    get:
      summary: Find webhooks
      description: Searches all webhooks available for a current user. Searches by
        name, resource, event, callback URL, or whether they are enabled. Returns
        a paged list of Webhooks
      operationId: findWebhooks
      x-api-path-slug: webhooks-get
      parameters:
      - in: query
        name: callback
        description: A callback URL
      - in: query
        name: enabled
        description: Specifies whether webhook is enabled
      - in: query
        name: event
        description: 'A name of event, available values: started, stopped, finished'
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name of a webhook
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: resource
        description: 'A name of a resource, available values: CccCampaign, CallBroadcast,
          TextBroadcast,  OutboundCall, OutboundText, InboundCall, InboundText, ContactList'
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    post:
      summary: Create a webhook
      description: 'Create a Webhook for notification in the CallFire system. Use
        the webhooks API to receive notifications of important CallFire events. Select
        the resource to listen to, and then choose the resource events to receive
        notifications on. When an event triggers, a POST will be made to the callback
        URL with a payload of notification information. Available resources and their
        events include ''CccCampaign'': [''started'', ''stopped'', ''finished''],
        ''CallBroadcast'': [''started'', ''stopped'', ''finished''], ''TextBroadcast'':
        [''started'', ''stopped'', ''finished''], ''OutboundCall'': [''finished''],
        ''InboundCall'': [''finished''], ''OutboundText'': [''finished''], ''InboundText'':
        [''finished''], ''ContactList'': [''validationFinished'', ''validationFailed''].
        Webhooks support secret token which is used as signing key to HmacSHA1 hash
        of json payload which is returned in ''X-CallFire-Signature'' header. This
        header can be used to verify callback POST is coming from CallFire. See [security
        guide](https://developers.callfire.com/security-guide.html)'
      operationId: createWebhook
      x-api-path-slug: webhooks-post
      parameters:
      - in: body
        name: body
        description: A webhook object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Webhooks
  /webhooks/resources:
    get:
      summary: Find webhook resources
      description: 'Searches for webhook resources. Available resources include ''CccCampaign'':
        [''started'', ''stopped'', ''finished''], ''CallBroadcast'': [''started'',
        ''stopped'', ''finished''], ''TextBroadcast'': [''started'', ''stopped'',
        ''finished''], ''OutboundCall'': [''finished''], ''InboundCall'': [''finished''],
        ''OutboundText'': [''finished''], ''InboundText'': [''finished''], ''ContactList'':
        [''validationFinished'', ''validationFailed'']'
      operationId: findWebhookResources
      x-api-path-slug: webhooksresources-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Resources
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