---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 0
info:
  title: ClimaCell Get Webhooks
  description: |-
    ### List all Webhooks
    Page through a list of all your Webhooks. You can specify the maximum number of results to be retuned, and from which result to start.
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