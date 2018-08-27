---
name: Gmail
x-slug: gmail
description: The Gmail API is a RESTful API that can be used to access Gmail mailboxes
  and send mail. For most web applications (including mobile apps), the Gmail API
  is the best choice for authorized access to a users Gmail data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Alias
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/gmail/apis.md
specificationVersion: "0.14"
apis:
- name: Gmail - Update Alias
  x-api-slug: useridsettingssendassendasemail-put
  description: |-
    Updates a send-as alias. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.

    Addresses other than the primary address for the account can only be updated by service account clients that have been delegated domain-wide authority.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/gmail/useridsettingssendassendasemail-put-openapi.md
- name: Gmail - Update Alias
  x-api-slug: useridsettingssendassendasemail-patch
  description: |-
    Updates a send-as alias. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.

    Addresses other than the primary address for the account can only be updated by service account clients that have been delegated domain-wide authority. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/gmail/useridsettingssendassendasemail-patch-openapi.md
- name: Gmail - Get Alias
  x-api-slug: useridsettingssendassendasemail-get
  description: Gets the specified send-as alias. Fails with an HTTP 404 error if the
    specified address is not a member of the collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/gmail/useridsettingssendassendasemail-get-openapi.md
- name: Gmail - Delete Alias
  x-api-slug: useridsettingssendassendasemail-delete
  description: |-
    Deletes the specified send-as alias. Revokes any verification that may have been required for using it.

    This method is only available to service account clients that have been delegated domain-wide authority.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/gmail/useridsettingssendassendasemail-delete-openapi.md
- name: Gmail - Create Alias
  x-api-slug: useridsettingssendas-post
  description: |-
    Creates a custom "from" send-as alias. If an SMTP MSA is specified, Gmail will attempt to connect to the SMTP service to validate the configuration before creating the alias. If ownership verification is required for the alias, a message will be sent to the email address and the resource's verification status will be set to pending; otherwise, the resource will be created with verification status set to accepted. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.

    This method is only available to service account clients that have been delegated domain-wide authority.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/gmail/useridsettingssendas-post-openapi.md
- name: Gmail - Send As Alias
  x-api-slug: useridsettingssendas-get
  description: Lists the send-as aliases for the specified account. The result includes
    the primary send-as address associated with the account as well as any custom
    "from" aliases.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Google APIs, Stack Network, Stack, Productivity, API Provider, Emails, Profiles,
    Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/gmail/useridsettingssendas-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://globalchange.gov.api.gallery.streamdata.io
- type: x-api-stack
  url: http://gmail.stack.network
- type: x-auth-scopes
  url: https://developers.google.com/gmail/api/auth/scopes
- type: x-authentication
  url: https://developers.google.com/gmail/api/auth/about-auth
- type: x-developer
  url: https://developers.google.com/gmail/api/
- type: x-documentation
  url: https://developers.google.com/gmail/api/v1/reference/
- type: x-twitter
  url: https://twitter.com/gmail
- type: x-website
  url: https://www.google.com/gmail/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---