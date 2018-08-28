---
name: Entertainment Express
x-slug: entertainment-express
description: Internet Video Archive (IVA) is a leading entertainment data company
  providing metadata, images and trailers/clips, for movie and TV content. With the
  launch of its award-winning Entertainment Express APIs, clients can easily access
  everything they need to create engaging content discovery experiences. By using
  Entertainment Express, clients can also connect to other services like movie showtimes
  and ticketing, content recommendations, content availability and TV channel line-ups.
  With over a million titles, episodes and over 150,000 videos available, IVA makes
  it easy for developers to integrate all the services they need at a very affordable
  price.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Find
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/entertainment-express/apis.md
specificationVersion: "0.14"
apis:
- name: Entertainment Express - Find a movie using third party ID.
  x-api-slug: findmovie-get
  description: "Use FindMovie with a third party ID like IMDB, TMDB, Gracenote, Tivo,
    etc. to find the corresponding movie in the IVA database.  For a full list of
    supported ID types see /Movies/AlternateIdTypes. \n\n\n\n`Recommendation: Use
    with small data sets or for a proof of concept. `"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/entertainment-express/findmovie-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/entertainment-express/findmovie-get-openapi.md
- name: Entertainment Express - Find a TV show using a third party ID.
  x-api-slug: findshow-get
  description: 'Use FindShow with a third party ID like IMDB, TMDB, Gracenote, Tivo,
    etc. to find the corresponding TV show in the IVA database. For a full list of
    supported ID types see /Shows/AlternateIdTypes. `Recommendation: Use with small
    data sets or for a proof of concept. `'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/entertainment-express/findshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/find/master/_listings/entertainment-express/findshow-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://emuseum.api.docs.api.gallery.streamdata.io
- type: x-api-stack
  url: http://entertainment.express.stack.network
- type: x-blog
  url: https://www.internetvideoarchive.com/blog/
- type: x-developer
  url: https://developer.iva-api.com/
- type: x-pricing
  url: https://www.internetvideoarchive.com/pricing/
- type: x-website
  url: https://www.internetvideoarchive.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---