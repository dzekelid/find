{
  "info": {
    "name": "Microsoft Graph API User Find Meeting Times",
    "_postman_id": "8b8a1047-8933-4489-8861-f0cf3dc1019d",
    "description": "user: findMeetingTimes Find meeting time suggestions based on organizer and attendee availability, and time or location constraints specified as parameters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "a4d3c603-9c33-4a0d-8eea-61e75c1681cb",
          "name": "User:FindMeetingTimes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id|userPrincipalName/findMeetingTimes"
              ],
              "variable": [
                {
                  "id": "id|userPrincipalName",
                  "value": "id|userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "{}",
                "description": "A string representing a specific time zone for the response, for example, \"Pacific Standard Time\"",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "user: findMeetingTimes Find meeting time suggestions based on organizer and attendee availability, and time or location constraints specified as parameters"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "54b96034-0ef0-467a-8a96-2a602beef65d"
            }
          ]
        }
      ]
    }
  ]
}