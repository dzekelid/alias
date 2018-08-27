swagger: "2.0"
x-collection-name: Gmail
x-complete: 1
info:
  title: Gmail
  version: 1.0.0
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
    get:
      summary: Get Alias
      description: Gets the specified send-as alias. Fails with an HTTP 404 error
        if the specified address is not a member of the collection.
      operationId: gmail.users.settings.sendAs.get
      x-api-path-slug: useridsettingssendassendasemail-get
      parameters:
      - in: path
        name: sendAsEmail
        description: The send-as alias to be retrieved
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Alias
    delete:
      summary: Delete Alias
      description: |-
        Deletes the specified send-as alias. Revokes any verification that may have been required for using it.

        This method is only available to service account clients that have been delegated domain-wide authority.
      operationId: gmail.users.settings.sendAs.delete
      x-api-path-slug: useridsettingssendassendasemail-delete
      parameters:
      - in: path
        name: sendAsEmail
        description: The send-as alias to be deleted
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Alias
  /{userId}/settings/sendAs:
    post:
      summary: Create Alias
      description: |-
        Creates a custom "from" send-as alias. If an SMTP MSA is specified, Gmail will attempt to connect to the SMTP service to validate the configuration before creating the alias. If ownership verification is required for the alias, a message will be sent to the email address and the resource's verification status will be set to pending; otherwise, the resource will be created with verification status set to accepted. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.

        This method is only available to service account clients that have been delegated domain-wide authority.
      operationId: gmail.users.settings.sendAs.create
      x-api-path-slug: useridsettingssendas-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Alias
    get:
      summary: Send As Alias
      description: Lists the send-as aliases for the specified account. The result
        includes the primary send-as address associated with the account as well as
        any custom "from" aliases.
      operationId: gmail.users.settings.sendAs.list
      x-api-path-slug: useridsettingssendas-get
      parameters:
      - in: path
        name: userId
        description: Users email address
      responses:
        200:
          description: OK
      tags:
      - Alias