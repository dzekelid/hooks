swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
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
    put:
      summary: Put Hooks
      description: ""
      operationId: putHooks.json
      x-api-path-slug: hooksid-json-put
      parameters:
      - in: body
        name: body
        description: Hook parameters
        schema:
          $ref: '#/definitions/holder'
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