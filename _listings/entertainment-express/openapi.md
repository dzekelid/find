swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
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