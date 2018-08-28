---
name: ClimaCell
x-slug: climacell
description: ClimaCell provides the most accurate weather data in the world by integrating
  proprietary data extracted from wireless networks and other new sensing technologies
  with data from traditional sensors. With 90% correlation to ground truth (vs. 50%
  using radar), it&rsquo;s the best you can get for your enterprise.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
x-kinRank: "9"
x-alexaRank: "617213"
tags: Hooks
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/climacell/apis.md
specificationVersion: "0.14"
apis:
- name: ClimaCell Get Webhooks
  x-api-slug: climacell
  description: |-
    ### List all Webhooks
    Page through a list of all your Webhooks. You can specify the maximum number of results to be retuned, and from which result to start.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//webhooks
  tags: Weather,Webhooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/climacell/webhooks-get-openapi.md
- name: ClimaCell Post Webhooks
  x-api-slug: climacell
  description: "### Create a Webhook\n\nCreates a new Webhook, and name it. The system
    attaches a unique ID to each webhook you create. This ID is used to refer to the
    webhook and manage it in the following \u200B```webhooks```\u200B API calls."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//webhooks
  tags: Weather,Webhooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/climacell/webhooks-post-openapi.md
- name: ClimaCell Get Webhooks Webhook
  x-api-slug: climacell
  description: |-
    ### Retrieve a Webhook

    Get a single Webhook with its information by specifying its ```webhook_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//webhooks/{webhook_id}
  tags: Weather,Webhooks,Webhook
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/climacell/webhookswebhook-id-get-openapi.md
- name: ClimaCell Put Webhooks Webhook
  x-api-slug: climacell
  description: "### Update a Webhook\n\nUpdates the name of a Webhook with a\u200B
    ```webhook_id```."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//webhooks/{webhook_id}
  tags: Weather,Webhooks,Webhook
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/climacell/webhookswebhook-id-put-openapi.md
- name: ClimaCell Delete Webhooks Webhook
  x-api-slug: climacell
  description: |-
    ### Delete a Webhook

    Removes a Webhook with its information by specifying its ```webhook_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//webhooks/{webhook_id}
  tags: Weather,Webhooks,Webhook
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/climacell/webhookswebhook-id-delete-openapi.md
- name: ClimaCell
  x-api-slug: climacell
  description: ClimaCell provides the most accurate weather data in the world by integrating
    proprietary data extracted from wireless networks and other new sensing technologies
    with data from traditional sensors. With 90% correlation to ground truth (vs.
    50% using radar), it&rsquo;s the best you can get for your enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Hooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/climacell/openapi.md
x-common:
- type: x-blog
  url: https://www.climacell.co/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/climacell
- type: x-developer
  url: https://www.climacell.co/api/
- type: x-email
  url: info@climacell.co
- type: x-email
  url: support@climacell.co
- type: x-email
  url: sales@climacell.co
- type: x-faq
  url: https://developer.climacell.co/FAQ
- type: x-github
  url: https://github.com/climacell
- type: x-pricing
  url: https://developer.climacell.co/
- type: x-privacy-policy
  url: https://www.climacell.co/privacy/
- type: x-terms-of-service
  url: https://www.climacell.co/terms-of-service/
- type: x-twitter
  url: https://twitter.com/WeatherRevealed
- type: x-website
  url: https://www.climacell.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---