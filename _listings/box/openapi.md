swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{USER_ID}/email_aliases/{EMAIL_ALIAS_ID}:
    delete:
      summary: Delete Email Alias
      description: Removes an email alias from a user.
      operationId: deleteUserEmailAlias
      x-api-path-slug: usersuser-idemail-aliasesemail-alias-id-delete
      parameters:
      - in: path
        name: EMAIL_ALIAS_ID
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
      - ""
      - Email
      - Aliases
      - Email
      - Alias