---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Get Hooks
  description: ""
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /hooks.json:
    get:
      summary: Get Hooks
      description: ""
      operationId: getHooks.json
      x-api-path-slug: hooks-json-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Hooks
      - Json
    post:
      summary: Post Hooks
      description: ""
      operationId: postHooks.json
      x-api-path-slug: hooks-json-post
      parameters:
      - in: body
        name: body
        description: Hook parameters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Hooks
      - Json
  /hooks/{id}.json:
    delete:
      summary: Delete Hooks
      description: ""
      operationId: deleteHooks.json
      x-api-path-slug: hooksid-json-delete
      parameters:
      - in: path
        name: id
        description: Id of the Hook
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Hooks
      - Id
      - Json
    get:
      summary: Get Hooks
      description: ""
      operationId: getHooks.json
      x-api-path-slug: hooksid-json-get
      parameters:
      - in: path
        name: id
        description: Id of the Hook
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Hooks
      - Id
      - Json
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