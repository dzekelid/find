{
  "info": {
    "name": "Clearbit Find Company by IP Address",
    "_postman_id": "c0a0bf68-7a8d-46ba-9481-79a69ef7340e",
    "description": "TODO: Add Description",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Business",
      "item": [
        {
          "id": "c22f3fbb-644f-4705-bec8-3a5a6e68a81d",
          "name": "SearchGet3",
          "request": {
            "url": "http://discovery.clearbit.com/v1/companies/search?domain=%7B%7D&email=%7B%7D&title=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "TODO: Add Description"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4a5ffce-89d2-4713-b532-16806a479b64"
            }
          ]
        },
        {
          "id": "683e6666-0b17-4019-b2de-b692d8db6054",
          "name": "FindGet2",
          "request": {
            "url": "http://discovery.clearbit.com/v1/companies/find?ip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "TODO: Add Description"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f5d33a0-a477-4429-879b-3020c08cdb3a"
            }
          ]
        }
      ]
    }
  ]
}