---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 1
info:
  title: 3Scale Account Management API
  description: the-api-for-managing-3scale-accounts-
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/api/webhooks/failures.xml:
    delete:
      summary: Webhooks Delete Failed Deliveries
      description: Webhooks delete failed deliveries.
      operationId: webhooks
      x-api-path-slug: adminapiwebhooksfailures-xml-delete
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: time
        description: Only failed webhook deliveries whose time is less or equal than
          the passed time are destroyed (if used)
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - ""
      - Failed
      - Deliveries
    get:
      summary: Webhooks List Failed Deliveries
      description: Webhooks list failed deliveries.
      operationId: webhooks
      x-api-path-slug: adminapiwebhooksfailures-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - List
      - Failed
      - Deliveries
---