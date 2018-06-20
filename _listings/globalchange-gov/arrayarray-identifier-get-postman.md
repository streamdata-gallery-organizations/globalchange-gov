{
  "info": {
    "name": "Global Change Information System API Get a representation of an array.",
    "_postman_id": "21adbedc-6780-41ce-8ca6-51dd37628cdd",
    "description": "Get JSON which represents the structure of an array.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activities",
      "item": [
        {
          "id": "8b27c075-3cb6-4e76-b1f2-744603e64e9e",
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
              "id": "4ce85894-4e6e-4a82-b02b-f3c34ffd6bbd"
            }
          ]
        }
      ]
    },
    {
      "name": "Representation",
      "item": [
        {
          "id": "26e1b76f-07f5-4ec9-9c2e-660810d3eb91",
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
              "id": "386fe0fd-d56f-4cbd-9b56-c60277167a7b"
            }
          ]
        },
        {
          "id": "07bff362-6df5-4536-98f8-1f85a2587d12",
          "name": "get-json-which-represents-the-structure-of-an-array",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "array/:array_identifier"
              ],
              "query": [
                {
                  "key": "with_gcmd",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "with_regions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "array_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an array."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18949a63-872a-4d57-afc8-7b50b5a041cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Arrays",
      "item": [
        {
          "id": "6d4164b5-0128-4008-abe4-cb5e35ea28dd",
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
              "id": "e4c12e2f-7826-4c92-b619-e5c6efd91c5d"
            }
          ]
        }
      ]
    }
  ]
}