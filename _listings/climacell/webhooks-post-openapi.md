---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 0
info:
  title: ClimaCell Post Webhooks
  description: "### Create a Webhook\n\nCreates a new Webhook, and name it. The system
    attaches a unique ID to each webhook you create. This ID is used to refer to the
    webhook and manage it in the following \u200B```webhooks```\u200B API calls."
  version: 1.0.0
host: api2.climacell.co
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
      summary: Get Webhooks
      description: |-
        ### List all Webhooks
        Page through a list of all your Webhooks. You can specify the maximum number of results to be retuned, and from which result to start.
      operationId: -list-all-webhookspage-through-a-list-of-all-your-webhooks-you-can-specify-the-maximum-number-of-res
      x-api-path-slug: webhooks-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of records to load
      - in: query
        name: offset
        description: The number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Webhooks
    post:
      summary: Post Webhooks
      description: "### Create a Webhook\n\nCreates a new Webhook, and name it. The
        system attaches a unique ID to each webhook you create. This ID is used to
        refer to the webhook and manage it in the following \u200B```webhooks```\u200B
        API calls."
      operationId: -create-a-webhookcreates-a-new-webhook-and-name-it-the-system-attaches-a-unique-id-to-each-webhook-y
      x-api-path-slug: webhooks-post
      parameters:
      - in: body
        name: webhook
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Weather
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