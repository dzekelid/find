{
  "info": {
    "name": "Entertainment Express Find a movie using third party ID.",
    "_postman_id": "d2c5c0e4-296d-4e86-808c-f3ace00fcbac",
    "description": "Use FindMovie with a third party ID like IMDB, TMDB, Gracenote, Tivo, etc. to find the corresponding movie in the IVA database.  For a full list of supported ID types see /Movies/AlternateIdTypes. \n\n\n\n`Recommendation: Use with small data sets or for a proof of concept. `",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "d1d21629-4fcb-4584-8c6e-c7bfdd2e8346",
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
              "id": "32d22cc6-6ee6-465c-94af-9a1aeb711e89"
            }
          ]
        }
      ]
    }
  ]
}