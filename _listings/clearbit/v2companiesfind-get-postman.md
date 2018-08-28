{
  "info": {
    "name": "Clearbit Domain Lookup",
    "_postman_id": "334e8d47-7fa7-411f-8937-15569e65e757",
    "description": "TODO: Add Description",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Business",
      "item": [
        {
          "id": "05cb562c-68c3-4f21-a67c-756b1d5e4abc",
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
              "id": "55cc313a-aae1-417e-8a10-95746d1c1544"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "b14d97b4-3ef8-4572-9d80-0b62278f2645",
          "name": "V2CompaniesFindGet",
          "request": {
            "url": "http://discovery.clearbit.com/v1/companies/v2/companies/find?domain=%7B%7D",
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
              "id": "a8f6af31-acde-43db-ad22-69cb1f16b1ed"
            }
          ]
        }
      ]
    }
  ]
}