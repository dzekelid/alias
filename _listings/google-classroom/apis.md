---
name: Google Classroom
x-slug: google-classroom
description: Google Classroom is mission control for your classes. As a free service
  for teachers and students, you can create classes, distribute assignments, send
  feedback, and see everything in one place. Instant. Paperless. Easy.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Alias
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/google-classroom/apis.md
specificationVersion: "0.14"
apis:
- name: Google Classroom - Get Course Work
  x-api-slug: v1coursescourseidcoursework-get
  description: |-
    Returns a list of course work that the requester is permitted to view.

    Course students may only view `PUBLISHED` course work. Course teachers
    and domain administrators may view all course work.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access
    the requested course or for access errors.
    * `INVALID_ARGUMENT` if the request is malformed.
    * `NOT_FOUND` if the requested course does not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/google-classroom/v1coursescourseidcoursework-get-openapi.md
- name: Google Classroom - Delete Alias
  x-api-slug: v1coursescourseidaliasesalias-delete
  description: |-
    Deletes an alias of a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to remove the
    alias or for access errors.
    * `NOT_FOUND` if the alias does not exist.
    * `FAILED_PRECONDITION` if the alias requested does not make sense for the
      requesting user or course (for example, if a user not in a domain
      attempts to delete a domain-scoped alias).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/google-classroom/v1coursescourseidaliasesalias-delete-openapi.md
- name: Google Classroom - Create Alias
  x-api-slug: v1coursescourseidaliases-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/google-classroom/v1coursescourseidaliases-post-openapi.md
- name: Google Classroom - Get Aliases
  x-api-slug: v1coursescourseidaliases-get
  description: |-
    Returns a list of aliases for a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access the
    course or for access errors.
    * `NOT_FOUND` if the course does not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alias/master/_listings/google-classroom/v1coursescourseidaliases-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.civic.information.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.classroom.stack.network
- type: x-button
  url: https://developers.google.com/classroom/guides/sharebutton
- type: x-developer
  url: https://developers.google.com/classroom/
- type: x-getting-started
  url: ""
- type: x-issues
  url: https://code.google.com/a/google.com/p/apps-api-issues/issues/list?can=2&q=label%3AAPI-Classroom
- type: x-website
  url: https://classroom.google.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---