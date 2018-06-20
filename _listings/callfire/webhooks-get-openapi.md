---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find webhooks
  description: Searches all webhooks available for a current user. Searches by name,
    resource, event, callback URL, or whether they are enabled. Returns a paged list
    of Webhooks
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