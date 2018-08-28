---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: |-
    Predix Intelligent Mapping For 'within' operator - find all points within an area.
    For 'nearest' operator - return the nearest point to the one specified.
    For 'lineIntersectsLine' - find all points of intersection between two linestrings.
  description: |-
    'Within' returns GeoGJSON of type FeatureCollection containing all GeoJSON features within the provided polygon.
    'Nearest' returns a FeatureCollection with the longitude and latitude of the nearest point.
    'LineIntersectsLine' returns a FeatureCollection containing all points of intersection as GeoJSON features.
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /
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