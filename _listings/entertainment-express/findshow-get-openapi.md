---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Find a TV show using a third party ID.
  description: 'Use FindShow with a third party ID like IMDB, TMDB, Gracenote, Tivo,
    etc. to find the corresponding TV show in the IVA database. For a full list of
    supported ID types see /Shows/AlternateIdTypes. `Recommendation: Use with small
    data sets or for a proof of concept. `'
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Find/Movie/:
    get:
      summary: Find a movie using third party ID.
      description: "Use FindMovie with a third party ID like IMDB, TMDB, Gracenote,
        Tivo, etc. to find the corresponding movie in the IVA database.  For a full
        list of supported ID types see /Movies/AlternateIdTypes. \n\n\n\n`Recommendation:
        Use with small data sets or for a proof of concept. `"
      operationId: FindMovie
      x-api-path-slug: findmovie-get
      parameters:
      - in: query
        name: Id
        description: Required third party ID of Movie
      - in: query
        name: IdType
        description: Required third party ID type of MovieAlternateId
      - in: query
        name: Includes
        description: List of additional objects to include in the movie object
      responses:
        200:
          description: OK
      tags:
      - Find
      - Movie
  /Find/Show/:
    get:
      summary: Find a TV show using a third party ID.
      description: 'Use FindShow with a third party ID like IMDB, TMDB, Gracenote,
        Tivo, etc. to find the corresponding TV show in the IVA database. For a full
        list of supported ID types see /Shows/AlternateIdTypes. `Recommendation: Use
        with small data sets or for a proof of concept. `'
      operationId: FindShow
      x-api-path-slug: findshow-get
      parameters:
      - in: query
        name: Id
        description: Required third party ID of Show
      - in: query
        name: IdType
        description: Required third party ID type of ShowAlternateId
      - in: query
        name: Includes
        description: List of additional objects to include in the show response
      responses:
        200:
          description: OK
      tags:
      - Find
      - Show
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