swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 1
info:
  title: Urban Airship
  description: the-urban-airships-api-powers-mobile-applications-with-push-rich-push-inapp-purchases-and-subscription-services-
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /push/scheduled/alias/{alias}:
    delete:
      summary: Delete Push Scheduled Alias Alias
      description: Deletes a scheduled notification alias.  If you attempt to schedule
        an aliased scheduled notification with an alias that already exists for your
        application, it will overwrite the existing one.
      operationId: push.scheduled.alias.alias.delete
      x-api-path-slug: pushscheduledaliasalias-delete
      parameters:
      - in: query
        name: alias
        description: Scheduled notification alias
      - in: path
        name: alias
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
      - Alias
      - Alias
    put:
      summary: Put Push Scheduled Alias Alias
      description: Changes a scheduled notification alias. Aliases for scheduled notifications
        are unique per Urban Airship application, so you might want to hash the aliases
        with a device ID or use some other mechanism to ensure uniqueness. The only
        other limit is that they must be 255 characters or less.
      operationId: push.scheduled.alias.alias.put
      x-api-path-slug: pushscheduledaliasalias-put
      parameters:
      - in: query
        name: alias
        description: Scheduled notification alias
      - in: path
        name: alias
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
      - Alias
      - Alias