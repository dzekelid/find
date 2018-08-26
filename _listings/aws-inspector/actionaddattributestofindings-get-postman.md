{
  "info": {
    "name": "AWS Inspector API Add Attributes To Findings",
    "_postman_id": "d5c87a87-3935-483b-b65b-5c23553c5fb8",
    "description": "Assigns attributes (key and value pairs) to the findings that are specified by the\n         ARNs of the findings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes To Findings",
      "item": [
        {
          "id": "5ce6879e-26e8-4757-80d7-2825608e727d",
          "name": "addAttributesToFindings",
          "request": {
            "url": "http://example.com/api/?Action=AddAttributesToFindings?attributes=attributes&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assigns attributes (key and value pairs) to the findings that are specified by the\n         ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8400365f-1e7c-4601-ab5d-d73b1c182a73"
            }
          ]
        }
      ]
    }
  ]
}