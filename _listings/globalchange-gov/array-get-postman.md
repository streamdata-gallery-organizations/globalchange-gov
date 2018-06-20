{
  "info": {
    "name": "Global Change Information System API List arrays.",
    "_postman_id": "8ad61baa-5757-4fc9-b0c9-81ca9d57e8df",
    "description": "List the arrays, 20 per page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activities",
      "item": [
        {
          "id": "8aa4acda-3ce3-46ce-a49c-962f081e9ffc",
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
              "id": "62cbdd03-738d-4fc7-a1ce-0b4b667c28fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Representation",
      "item": [
        {
          "id": "2593edaa-05c7-4e7b-b5af-d56e3d3e681e",
          "name": "get-json-which-represents-the-structure-of-an-activity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "activity/:activity_identifier"
              ],
              "variable": [
                {
                  "id": "activity_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f132b253-a372-45e5-9829-c584666b746b"
            }
          ]
        }
      ]
    },
    {
      "name": "Arrays",
      "item": [
        {
          "id": "864afc58-c14e-4105-a032-39a5eb351f44",
          "name": "list-the-arrays-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/array?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the arrays, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86021af5-4495-468f-b890-b49aef7d8f55"
            }
          ]
        }
      ]
    }
  ]
}