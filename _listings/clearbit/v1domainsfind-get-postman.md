{
  "info": {
    "name": "Clearbit Company Name to Domain",
    "_postman_id": "b6294a9a-fe18-4bbd-b04d-8fb8cb068132",
    "description": "TODO: Add Description",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Business",
      "item": [
        {
          "id": "aa5198a1-21ad-4a05-9d9f-107054df05cc",
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
              "id": "e79de3aa-f437-4a32-af8c-18e84176182e"
            }
          ]
        },
        {
          "id": "aa615249-87f5-4d71-82c1-ff9286ae492e",
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
              "id": "089134e2-0aae-4d7f-8c02-b9f6b4ad93e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "5a38ce15-1e7f-412c-95cf-8dcca9dfbccf",
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
              "id": "b373b7a6-ce6d-444e-b647-99830e2906d3"
            }
          ]
        },
        {
          "id": "9f5f012d-b630-42c6-b74c-3827c914b147",
          "name": "V1DomainsFindGet",
          "request": {
            "url": "http://discovery.clearbit.com/v1/companies/v1/domains/find?name=%7B%7D",
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
              "id": "a72d6d41-bf4e-40b2-8cdd-f01b68f7c799"
            }
          ]
        }
      ]
    }
  ]
}