{
  "info": {
    "name": "Global Change Information System API List activities.",
    "_postman_id": "0a2359f5-ad53-4c8e-99b8-c06985588c9a",
    "description": "List the activities, 20 per page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activities",
      "item": [
        {
          "id": "edade58d-c64c-4e38-8dca-2dc68ea5e72b",
          "name": "list-the-activities-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/activity?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activities, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d048431-2de8-4023-8634-3cdbd1977c90"
            }
          ]
        }
      ]
    }
  ]
}