---
swagger: "2.0"
x-collection-name: Gmail
x-complete: 0
info:
  title: Gmail Update Alias
  description: |-
    Updates a send-as alias. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.

    Addresses other than the primary address for the account can only be updated by service account clients that have been delegated domain-wide authority. This method supports patch semantics.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /gmail/v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{userId}/settings/sendAs/{sendAsEmail}:
    put:
      summary: Update Alias
      description: |-
        Updates a send-as alias. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.

        Addresses other than the primary address for the account can only be updated by service account clients that have been delegated domain-wide authority.
      operationId: gmail.users.settings.sendAs.update
      x-api-path-slug: useridsettingssendassendasemail-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: sendAsEmail
        description: The send-as alias to be updated
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Alias
    patch:
      summary: Update Alias
      description: |-
        Updates a send-as alias. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.

        Addresses other than the primary address for the account can only be updated by service account clients that have been delegated domain-wide authority. This method supports patch semantics.
      operationId: gmail.users.settings.sendAs.patch
      x-api-path-slug: useridsettingssendassendasemail-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: sendAsEmail
        description: The send-as alias to be updated
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Alias
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