---
swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
---