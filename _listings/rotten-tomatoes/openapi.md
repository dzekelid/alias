swagger: "2.0"
x-collection-name: Rotten Tomatoes
x-complete: 1
info:
  title: Rotten Tomatoes
  description: test-our-api-services-using-io-docs-
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