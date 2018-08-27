---
swagger: "2.0"
x-collection-name: Rotten Tomatoes
x-complete: 0
info:
  title: Rotten Tomatoes Get Movie Alias
  description: Get movie alias.json.
  contact:
    name: Mike Ralphson
    url: https://github.com/mermade/mashery2openapi
    email: mike.ralphson@gmail.com
  version: "1.0"
host: api.rottentomatoes.com
basePath: /api/public/v1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /movie_alias.json:
    get:
      summary: Get Movie Alias
      description: Get movie alias.json.
      operationId: getMovieAlias.json
      x-api-path-slug: movie-alias-json-get
      parameters:
      - in: query
        name: id
        description: Movie ID
      - in: query
        name: type
        description: Only supports imdb lookup at this time
      responses:
        200:
          description: OK
      tags:
      - Movie
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