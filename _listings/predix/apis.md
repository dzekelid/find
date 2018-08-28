---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Find
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: |-
    Intelligent Mapping - For 'within' operator - find all points within an area.
    For 'nearest' operator - return the nearest point to the one specified.
    For 'lineIntersectsLine' - find all points of intersection between two linestrings.
  x-api-slug: v1collectionscollectionnamespatialquery-post
  description: |-
    'Within' returns GeoGJSON of type FeatureCollection containing all GeoJSON features within the provided polygon.
    'Nearest' returns a FeatureCollection with the longitude and latitude of the nearest point.
    'LineIntersectsLine' returns a FeatureCollection containing all points of intersection as GeoJSON features.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/predix/v1collectionscollectionnamespatialquery-post-openapi.md
- name: VIEWS - Find all instances of the Deck matched by filter.
  x-api-slug: decks-get
  description: Find all instances of the deck matched by filter..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////v1
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/predix/decks-get-openapi.md
- name: VIEWS - Find a Deck instance by id.
  x-api-slug: decksid-get
  description: Find a deck instance by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////v1
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/predix/decksid-get-openapi.md
- name: VIEWS - Find all instances of the Card matched by filter.
  x-api-slug: cards-get
  description: Find all instances of the card matched by filter..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////v1
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/predix/cards-get-openapi.md
- name: VIEWS - Find a Card instance by id.
  x-api-slug: cardsid-get
  description: Find a card instance by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////v1
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/predix/cardsid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---