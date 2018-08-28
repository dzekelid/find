---
name: HERE
x-slug: here
description: HERE Technologies enables people, enterprises and cities around the world
  to harness the power of location and create innovative solutions that make our lives
  safer and more efficient. We transform information from devices, vehicles, infrastructure
  and...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
x-kinRank: "7"
x-alexaRank: "3011"
tags: Find
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/apis.md
specificationVersion: "0.14"
apis:
- name: Custom Location Extension API - Find Locations within a Bounding Box
  x-api-slug: bbox-get
  description: |-
    *Request a list of user-defined locations within a defined area*

    The request uses the `bbox` endpoint, and the bounding box is specified by adding the `bbox` parameter to the request URL.



    * **layerId**  `text`
     \- Unique indicator used to retrieve a dataset

    * **bbox**  `bbox`
     \- Restricts results to be found within this bounding box

    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://customlocation.cit.api.here.com//v1/search
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/bbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/bbox-get-openapi.md
- name: Custom Location Extension API - Find the Five Nearest Locations
  x-api-slug: proximity-get
  description: |-
    *Request a list of user-defined locations within a circle around a fixed point*

    The search uses the `proximity` endpoint. The definition of the location and limit of the search is specified using  `coord` and `radius` parameters, and the number of results returned limited by adding the `limit` parameter to the request URL.



    * **layerId**  `text`
     \- Unique indicator used to retrieve a dataset

    * **coord**  `latlng`
     \- Center of the proximity search

    * **radius**  `number`
     \- width of the search corridor

    * **limit**  `number`
     \- The limit of the number of items contained in the response.

    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://customlocation.cit.api.here.com//v1/search
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/proximity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/proximity-get-openapi.md
- name: Custom Location Extension API - Find Locations along a pre-defined Route
  x-api-slug: routecorridor-get
  description: |-
    *Request a list of user-defined locations along a pre-defined route*

    The route has been pre-calculated and the `routeid` has already been acquired from a previous routing request. A route-based corridor search is requested using the `corridor` endpoint and by adding the `routeid` parameter to the request URL, along with a corridor `width`.



    * **layerId**  `text`
     \- Unique indicator used to retrieve a dataset

    * **routeId**  `text`
     \- A <b>previously</b> calculated routeId

    * **radius**  `number`
     \- Width of the search corridor

    * **limit**  `number`
     \- The limit of the number of items contained in the response.

    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://customlocation.cit.api.here.com//v1/search
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/routecorridor-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/routecorridor-get-openapi.md
- name: Custom Location Extension API - Find Locations using Corridor
  x-api-slug: corridor-get
  description: |-
    *Request a list of user-defined locations near to a given corridor*

    The route corridor consists of a series of latitude, longitude pairs defining the waypoints of a route, along with a defined width. A corridor search is requested using the `corridor` endpoint and by adding a series of comma delimited latitude, longitude waypoints to the `route` parameter of the request URL, along with a `radius` for the search.



    * **layerId**  `text`
     \- Unique indicator used to retrieve a dataset

    * **route**  `text`
     \- A type of spatial filter. The corridor is defined by its path and width. The path is a line along the center of the corridor represented by a series of latitude/longitude pairs. Corridor width is given in meters.

    * **radius**  `number`
     \- width of the search corridor

    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://customlocation.cit.api.here.com//v1/search
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/corridor-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/corridor-get-openapi.md
- name: Public Transport API - Find Stations by Name
  x-api-slug: searchby-name-json-get
  description: "*Request a list of public transit stations based on name*\n\nA station
    search request can be made using the `search/by_name.json` endpoint and adding
    the `name` parameter. The focal point of the search is defined using the `x` and
    `y` parameters. The number of results can be further restricted by `max `and the
    `radius `parameters.\n  \n\n\n\n* **x**  `number`\n \\- The longitude of the center
    point of your search.    e.g. `13.377`\n\n* **y**  `number`\n \\- The latitude
    of the center point of your search.    e.g. `52.515`\n\n* **name**  `text`\n \\-
    Specifies the name or a part of the name of the station to search for and can
    be one word, multiple words or partial word separated by either comma or space.\n\n*
    **app_id**  `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for the
    authentication of the client application.    You must include an app_code and
    app_code with every request.\n\n* **app_code**  `text`\n \\- A 20 bytes Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an app_code and app_code with every request.\n\n* **max**
    \ `number`\n \\- Specifies the maximum number of stations/stops included in the
    response.\n  The minimum value is 1 and the maximum value is not limited.\n  The
    default value is 5.     \n\n* **method**  `enum`\n \\- Specifies if the matching
    method is *fuzzy* or *strict*.\n  The default value is *fuzzy*.\n    * fuzzy -
    search for stations with the name having similar sounding and/or similar spelling
    to the names requested\n    * strict - search for stations with the name exactly
    matching the names requested or contains it as its part.\n\n   Valid values are
    : `fuzzy`, `strict`\n\n* **radius**  `number`\n \\- Specifies a radius in meters
    when combined with a center point defines the area of the search. The minimum
    value is 0 and the maximum value is not limited.\n  The default value is 20000km."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/searchby-name-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/searchby-name-json-get-openapi.md
- name: Public Transport API - Find Stations by ID
  x-api-slug: searchby-stopids-json-get
  description: "*Request details of a specific transit station based on a previous
    request*\n\nStation details are requested using the `search/by_stopids.json` endpoint
    and appending a comma delimited list of `stop-ids` to the request URL. Usually,
    the request to this endpoint will be called after making a station search request,
    to obtain a list of stations Ids.\n  \n\n\n\n* **stopIds**  `text`\n \\- Specifies
    a list of stopIds separated by comma. Each stopId must contain at least 6 characters
    and must not exceed a maximum of 1000 characters.     The format of a station
    Id is 123456789#100. Only the first 9-digits are mandatory and if the full Id
    is to be used, the `#` character must be encoded as `%23`.      \n\n* **lang**
    \ `text`\n \\- A language of the response. \n\n* **app_id**  `text`\n \\- A 20
    bytes Base64 URL-safe encoded string used for the authentication of the client
    application.    You must include an app_code and app_code with every request.\n\n*
    **app_code**  `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for
    the authentication of the client application.    You must include an app_code
    and app_code with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/searchby-stopids-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/searchby-stopids-json-get-openapi.md
- name: Public Transport API - Find Stations Nearby
  x-api-slug: searchby-geocoord-json-get
  description: "*Request a list of public transit stations within a given geo-location.*\n\nTo
    find the nearest stations use the `search/by_geocoord.json` endpoint specifying
    a center point using the `x` and `y` parameters and a search radius in meters
    using the `radius` parameter. `Max` value can also be used to restrict the number
    of results shown in the response.\n\n\n\n* **y**  `number`\n \\- The latitude
    of the center point of your search.    e.g. `52.515`\n\n* **x**  `number`\n \\-
    The longitude of the center point of your search.    e.g. `13.377`\n\n* **radius**
    \ `number`\n \\- Specifies a radius in meters when combined with the geo-coordinates
    defines the area of the search. The default value is 500m.\n\n* **app_id**  `text`\n
    \\- A 20 bytes Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an app_code and app_code with every request.\n\n*
    **app_code**  `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for
    the authentication of the client application.    You must include an app_code
    and app_code with every request.\n\n* **max**  `number`\n \\- Specifies the maximum
    number of stations/stops included in the response. \n          The default value
    is 5. The minimum value is 1 and the maximum value is not limited."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/searchby-geocoord-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/searchby-geocoord-json-get-openapi.md
- name: Public Transport API - Find Transit Coverage in Cities Nearby
  x-api-slug: coveragev1city-json-get
  description: "*Request a list of transit operators available in cities nearby*\n\nCity
    coverage can be found using the `coverage/v1/city.json` endpoint. The `x` and
    `y` parameters specify the location of the search.\n  The response also includes
    the number of transit lines and transit stops available for each city.\n  \n\n\n\n*
    **x**  `number`\n \\- The longitude of the center point of your search.    e.g.
    `13.377`\n\n* **y**  `number`\n \\- The latitude of the center point of your search.
    \   e.g. `52.515`\n\n* **chinaconfig**  `enum`\n \\- A switch that allows grouping
    results from Taiwan\ntogether with results from China.    When enabled, Taiwan
    will appear as part of China.    \n\n    Valid values are : `0` - disabled, `1`
    - enabled\n\n* **radius**  `number`\n \\- Specifies a radius in meters when combined
    with a center point defines the area of the search.\n\n* **app_id**  `text`\n
    \\- A 20 bytes Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an app_code and app_code with every request.\n\n*
    **app_code**  `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for
    the authentication of the client application.    You must include an app_code
    and app_code with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/coveragev1city-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/here/coveragev1city-json-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://developer.here.com/blog/feed
- type: x-github
  url: https://github.com/heremaps
- type: x-postman-collection
  url: https://github.com/heremaps/postman-collections
- type: x-api-gallery
  url: http://healthcare.gov.api.gallery.streamdata.io
- type: x-api-stack
  url: http://here.stack.network
- type: x-blog
  url: https://developer.here.com/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/here-inc
- type: x-developer
  url: https://developer.here.com
- type: x-email
  url: dirk.popp@here.com
- type: x-email
  url: sebastian.kurme@here.com
- type: x-email
  url: jordan.stark@here.com
- type: x-email
  url: amy.stupavsky@here.com
- type: x-email
  url: minna.laub@here.com
- type: x-email
  url: stefanie.sirc@here.com
- type: x-email
  url: rachel.kuta@here.com
- type: x-email
  url: laurel.davis-lyons@here.com
- type: x-email
  url: linda.bradley@here.com
- type: x-email
  url: press@here.com
- type: x-twitter
  url: https://twitter.com/here
- type: x-website
  url: https://here.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---