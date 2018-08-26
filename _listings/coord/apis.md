---
name: Coord
x-slug: coord
description: Coord is a mobility company that creates seamless mobility and self-driving
  experiences today through deep integrations. The company offers bike-share API,
  Curbs API, Tolls API, Routing API and etc.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
x-kinRank: "7"
x-alexaRank: "1035226"
tags: Find
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/apis.md
specificationVersion: "0.14"
apis:
- name: Curb Search API - Find the rules for all curbs within a bounding box.
  x-api-slug: byboundsall-rules-get
  description: Find the rules for all curbs within a bounding box..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/curbs
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/byboundsall-rules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/byboundsall-rules-get-openapi.md
- name: Curb Search API - Find the rules for all curbs within a bounding box at a
    particular time.
  x-api-slug: byboundstime-rules-get
  description: Find the rules for all curbs within a bounding box at a particular
    time..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/curbs
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/byboundstime-rules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/byboundstime-rules-get-openapi.md
- name: Curb Search API - Find the rules on single curb.
  x-api-slug: bycurbidall-rules-get
  description: Find the rules on single curb..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/curbs
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/bycurbidall-rules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/bycurbidall-rules-get-openapi.md
- name: Curb Search API - Find the rules on a single curb at a certain time.
  x-api-slug: bycurbidtime-rules-get
  description: Find the rules on a single curb at a certain time..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/curbs
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/bycurbidtime-rules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/bycurbidtime-rules-get-openapi.md
- name: Curb Search API - Find the rules for curbs near a location.
  x-api-slug: bylocationall-rules-get
  description: |-
    Find all of the curbs within a given radius of a particular point, and return all of their
    rules across all times of day, days of the week, times of year, etc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/curbs
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/bylocationall-rules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/bylocationall-rules-get-openapi.md
- name: Curb Search API - Find the rules for curbs near a location at a certain time.
  x-api-slug: bylocationtime-rules-get
  description: |-
    Find the rules for a given curb at a given time and on a given day. You can also use this
    to find all of the places that it is possible to perform a given action (for instance, find
    all the loading zones, or everywhere with two-hour parking).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/curbs
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/bylocationtime-rules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/coord/bylocationtime-rules-get-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/coord
- type: x-blog-rss
  url: https://medium.com/feed/coord
- type: x-openapi
  url: https://jsapi.apiary.io/apis/coordprodsearchtolls.source
- type: x-api-gallery
  url: http://convertapi.api.gallery.streamdata.io
- type: x-api-stack
  url: http://coord.stack.network
- type: x-developer
  url: https://coord.co/docs/
- type: x-pricing
  url: https://coord.co/#pricing
- type: x-twitter
  url: https://twitter.com/coordcity
- type: x-website
  url: https://coord.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---