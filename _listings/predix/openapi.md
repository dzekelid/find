swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/collections/{collectionName}/spatial-query:
    post:
      summary: |-
        For 'within' operator - find all points within an area.
        For 'nearest' operator - return the nearest point to the one specified.
        For 'lineIntersectsLine' - find all points of intersection between two linestrings.
      description: |-
        'Within' returns GeoGJSON of type FeatureCollection containing all GeoJSON features within the provided polygon.
        'Nearest' returns a FeatureCollection with the longitude and latitude of the nearest point.
        'LineIntersectsLine' returns a FeatureCollection containing all points of intersection as GeoJSON features.
      operationId: within-returns-geogjson-of-type-featurecollection-containing-all-geojson-features-within-the-provide
      x-api-path-slug: v1collectionscollectionnamespatialquery-post
      parameters:
      - in: body
        name: body
        description: For within query - a geojson polygon which we wish to search
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: operator
        description: The type of spatial query
      responses:
        200:
          description: OK
      tags:
      - For
      - Within
      - Operator
      - '-'
      - Find
      - ""
      - Points
      - Within
      - Area
      - For
      - Nearest
      - Operator
      - '-'
      - Return
      - Nearest
      - Point
      - To
      - Specified
      - For
      - LineIntersectsLine
      - '-'
      - Find
      - ""
      - Points
      - Of
      - Intersection
      - Between
      - Two
      - Linestrings
  /decks:
    get:
      summary: Find all instances of the Deck matched by filter.
      description: Find all instances of the deck matched by filter..
      operationId: getDecks
      x-api-path-slug: decks-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Deck
      - Matched
      - By
      - Filter
  /decks/{id}:
    get:
      summary: Find a Deck instance by id.
      description: Find a deck instance by id..
      operationId: getDecks
      x-api-path-slug: decksid-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields and include
      - in: path
        name: id
        description: Deck id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Deck
      - Instance
      - By
      - Id
  /cards:
    get:
      summary: Find all instances of the Card matched by filter.
      description: Find all instances of the card matched by filter..
      operationId: getCards
      x-api-path-slug: cards-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Card
      - Matched
      - By
      - Filter
  /cards/{id}:
    get:
      summary: Find a Card instance by id.
      description: Find a card instance by id..
      operationId: getCards
      x-api-path-slug: cardsid-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields and include
      - in: path
        name: id
        description: Card id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Card
      - Instance
      - By
      - Id