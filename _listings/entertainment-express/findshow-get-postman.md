{
  "info": {
    "name": "Entertainment Express Find a TV show using a third party ID.",
    "_postman_id": "92c5ce71-c364-4ad5-81df-5563dc9da344",
    "description": "Use FindShow with a third party ID like IMDB, TMDB, Gracenote, Tivo, etc. to find the corresponding TV show in the IVA database. For a full list of supported ID types see /Shows/AlternateIdTypes. `Recommendation: Use with small data sets or for a proof of concept. `",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "7fcbb692-c160-4f16-8f57-ebe41e4f4088",
          "name": "FindMovie",
          "request": {
            "url": "http://ee.iva-api.com/Find/Movie/?Id=%7B%7D&IdType=%7B%7D&Includes=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use FindMovie with a third party ID like IMDB, TMDB, Gracenote, Tivo, etc. to find the corresponding movie in the IVA database.  For a full list of supported ID types see /Movies/AlternateIdTypes. \n\n\n\n`Recommendation: Use with small data sets or for a proof of concept. `"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6d08417-9222-42bf-85db-a4e0309d2120"
            }
          ]
        },
        {
          "id": "e19ff765-0c9b-43e6-b144-ededf29ad486",
          "name": "FindShow",
          "request": {
            "url": "http://ee.iva-api.com/Find/Show/?Id=%7B%7D&IdType=%7B%7D&Includes=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use FindShow with a third party ID like IMDB, TMDB, Gracenote, Tivo, etc. to find the corresponding TV show in the IVA database. For a full list of supported ID types see /Shows/AlternateIdTypes. `Recommendation: Use with small data sets or for a proof of concept. `"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe8b85cf-3931-4976-b5fc-201990cdb90e"
            }
          ]
        }
      ]
    }
  ]
}