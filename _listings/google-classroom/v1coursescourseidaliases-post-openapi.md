---
swagger: "2.0"
x-collection-name: Google Classroom
x-complete: 0
info:
  title: Google Classroom API Create Alias
  description: |-
    Creates an alias for a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to create the
    alias or for access errors.
    * `NOT_FOUND` if the course does not exist.
    * `ALREADY_EXISTS` if the alias already exists.
    * `FAILED_PRECONDITION` if the alias requested does not make sense for the
      requesting user or course (for example, if a user not in a domain
      attempts to access a domain-scoped alias).
  contact:
    name: Google
    url: https://google.com
  version: v1
host: classroom.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/courses/{courseId}/courseWork:
    get:
      summary: Get Course Work
      description: |-
        Returns a list of course work that the requester is permitted to view.

        Course students may only view `PUBLISHED` course work. Course teachers
        and domain administrators may view all course work.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access
        the requested course or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course does not exist.
      operationId: classroom.courses.courseWork.list
      x-api-path-slug: v1coursescourseidcoursework-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: query
        name: courseWorkStates
        description: Restriction on the work status to return
      - in: query
        name: orderBy
        description: Optional sort ordering for results
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call,indicating
          that the subsequent page of results should be returned
      responses:
        200:
          description: OK
      tags:
      - Alias
  /v1/courses/{courseId}/aliases/{alias}:
    delete:
      summary: Delete Alias
      description: |-
        Deletes an alias of a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to remove the
        alias or for access errors.
        * `NOT_FOUND` if the alias does not exist.
        * `FAILED_PRECONDITION` if the alias requested does not make sense for the
          requesting user or course (for example, if a user not in a domain
          attempts to delete a domain-scoped alias).
      operationId: classroom.courses.aliases.delete
      x-api-path-slug: v1coursescourseidaliasesalias-delete
      parameters:
      - in: path
        name: alias
        description: Alias to delete
      - in: path
        name: courseId
        description: Identifier of the course whose alias should be deleted
      responses:
        200:
          description: OK
      tags:
      - Alias
  /v1/courses/{courseId}/aliases:
    post:
      summary: Create Alias
      description: |-
        Creates an alias for a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to create the
        alias or for access errors.
        * `NOT_FOUND` if the course does not exist.
        * `ALREADY_EXISTS` if the alias already exists.
        * `FAILED_PRECONDITION` if the alias requested does not make sense for the
          requesting user or course (for example, if a user not in a domain
          attempts to access a domain-scoped alias).
      operationId: classroom.courses.aliases.create
      x-api-path-slug: v1coursescourseidaliases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course to alias
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