---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Find a Deck instance by id.
  version: 1.0.0
  description: Find a deck instance by id..
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