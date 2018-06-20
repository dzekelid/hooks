---
name: GitHub
x-slug: github
description: With a community of more than 10 million people, developers can discover,
  use and contribute to over 24 million projects using a powerful, collaborative workflow.    Whether
  using GitHub.com or your own instance of GitHub Enterprise, you can integrate ...
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "70"
tags: Hooks
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: Github Get Repos Owner Repo Hooks
  x-api-slug: github
  description: Get list of hooks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/hooks
  tags: Repos, Owner, Repo, Hooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohooks-get-openapi.md
- name: Github Add Repos Owner Repo Hooks
  x-api-slug: github
  description: Create a hook.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/hooks
  tags: Repos, Owner, Repo, Hooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohooks-post-openapi.md
- name: Github Delete Repos Owner Repo Hooks Hook
  x-api-slug: github
  description: Delete a hook.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/hooks/{hookId}
  tags: Repos, Owner, Repo, Hooks, Hook
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohookshookid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohookshookid-delete-openapi.md
- name: Github Get Repos Owner Repo Hooks Hook
  x-api-slug: github
  description: Get single hook.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/hooks/{hookId}
  tags: Repos, Owner, Repo, Hooks, Hook
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohookshookid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohookshookid-get-openapi.md
- name: Github Patch Repos Owner Repo Hooks Hook
  x-api-slug: github
  description: Edit a hook.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/hooks/{hookId}
  tags: Repos, Owner, Repo, Hooks, Hook
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohookshookid-patch-openapi.md
- name: Github Add Repos Owner Repo Hooks Hook Tests
  x-api-slug: github
  description: |-
    Test a push hook.
    This will trigger the hook with the latest push to the current repository
    if the hook is subscribed to push events. If the hook is not subscribed
    to push events, the server will respond with 204 but no test POST will
    be generated.
    Note: Previously /repos/:owner/:repo/hooks/:id/tes
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/hooks/{hookId}/tests
  tags: Repos, Owner, Repo, Hooks, Hook, Tests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohookshookidtests-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/reposownerrepohookshookidtests-post-openapi.md
- name: Github
  x-api-slug: github
  description: With a community of more than 10 million people, developers can discover,
    use and contribute to over 24 million projects using a powerful, collaborative
    workflow.    Whether using GitHub.com or your own instance of GitHub Enterprise,
    you can integrate ...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Hooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/github/openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---