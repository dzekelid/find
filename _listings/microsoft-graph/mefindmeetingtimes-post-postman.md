{
  "info": {
    "name": "Microsoft Graph API User Find Meeting Times",
    "_postman_id": "50e36712-7f0c-46cb-b89f-aaac4f447757",
    "description": "user: findMeetingTimes Find meeting time suggestions based on organizer and attendee availability, and time or location constraints specified as parameters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "7d3c36a1-ae2b-4201-ae6c-1f4a99a8f9e9",
          "name": "User:FindMeetingTimes",
          "request": {
            "url": "http://graph.microsoft.com/me/findMeetingTimes",
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
              "id": "a4d41944-f834-4d9d-8d17-53edd562bbff"
            }
          ]
        }
      ]
    }
  ]
}