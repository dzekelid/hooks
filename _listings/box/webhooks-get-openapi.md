---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get Webhooks
  description: |-
    Returns all defined webhooks for the requesting application and user, up to the limit. If no limit is supplied then Box uses the default limit of 100.
    If more than limit webhooks are defined then Box returns the webhooks in batches. When the results are batched, Box sends limit webhooks along with a next_marker field in the response object. The value of the next_marker field is a marker string that you can use in later requests to tell Box which batch to send next.
    When you send a request that includes a marker string, Box sends the next batch of webhooks, beginning after the last webhook of the previous batch. When the response contains the last of the defined webhooks, Box omits the next_marker field from its response.
    You can use limit and marker together with the marker string returned in the next_marker field to paginate lists of webhooks.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /webhooks:
    post:
      summary: Create Webhook
      description: Create Webhook
      operationId: createWebhook
      x-api-path-slug: webhooks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Webhooks
    get:
      summary: Get Webhooks
      description: |-
        Returns all defined webhooks for the requesting application and user, up to the limit. If no limit is supplied then Box uses the default limit of 100.
        If more than limit webhooks are defined then Box returns the webhooks in batches. When the results are batched, Box sends limit webhooks along with a next_marker field in the response object. The value of the next_marker field is a marker string that you can use in later requests to tell Box which batch to send next.
        When you send a request that includes a marker string, Box sends the next batch of webhooks, beginning after the last webhook of the previous batch. When the response contains the last of the defined webhooks, Box omits the next_marker field from its response.
        You can use limit and marker together with the marker string returned in the next_marker field to paginate lists of webhooks.
      operationId: getWebhooks
      x-api-path-slug: webhooks-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of webhooks to return per page
      - in: query
        name: marker
        description: A marker string returned by Box if the result contains less than
          the full number of webhooks that are defined
      responses:
        200:
          description: OK
      tags:
      - Documents
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