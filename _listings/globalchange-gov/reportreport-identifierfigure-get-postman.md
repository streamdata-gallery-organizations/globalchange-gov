{
  "info": {
    "name": "Global Change Information System API List figures in a report.",
    "_postman_id": "dac0f40f-b425-4ad7-9af4-87bfb7b6bfe2",
    "description": "List the figures in a report, 20 per page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activities",
      "item": [
        {
          "id": "6e443e7c-056c-42ab-9545-2722007ef914",
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
              "id": "b9f839a7-abcf-48ba-bd49-48e6039895ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Representation",
      "item": [
        {
          "id": "d146c1c7-f9e6-4958-a576-0cd156a62697",
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
              "id": "9d1b4ac8-d1bc-4203-af73-cd3051539efa"
            }
          ]
        },
        {
          "id": "bb224907-d4b9-44ab-a544-ea400cb9a249",
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
              "id": "d0bea171-e1cc-4f7a-9f38-8abd0c46302c"
            }
          ]
        },
        {
          "id": "75cc0d2b-be30-42dd-bb80-e8492f309145",
          "name": "get-json-which-represents-the-structure-of-an-article",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "article/:article_identifier"
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
                  "id": "article_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an article."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bbccb90-225f-4a33-9f19-2f62c9e8a59b"
            }
          ]
        },
        {
          "id": "42739011-34d4-4788-ab97-1c0a778fa6c9",
          "name": "get-json-which-represents-the-structure-of-a-book",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "book/:book_identifier"
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
                  "id": "book_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a book."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27bec571-6ddf-44e4-bb2c-c6d301670410"
            }
          ]
        },
        {
          "id": "a7a7a399-32b9-4999-81dc-998e9dd2bd24",
          "name": "get-json-which-represents-the-structure-of-a-dataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "dataset/:dataset_identifier"
              ],
              "variable": [
                {
                  "id": "dataset_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "401b465d-e91a-4c34-aca6-765435a8e41e"
            }
          ]
        },
        {
          "id": "07659273-ab3f-42db-b9e3-23ca88ad8df7",
          "name": "get-json-which-represents-the-structure-of-a-file",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "file/:file_identifier"
              ],
              "variable": [
                {
                  "id": "file_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96edfec8-594c-4b38-81f7-5fd1133b0e52"
            }
          ]
        },
        {
          "id": "0277f90f-a041-4e6e-aa8f-b501c1f13743",
          "name": "get-json-which-represents-the-structure-of-a-gcmd-keyword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "gcmd_keyword/:gcmd_keyword_identifier"
              ],
              "variable": [
                {
                  "id": "gcmd_keyword_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a GCMD keyword."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9589c38-b467-4ed3-89d9-ed3f1678b33d"
            }
          ]
        },
        {
          "id": "36284403-4185-4759-915a-132134cc7c47",
          "name": "get-json-which-represents-the-structure-of-a-generic-publication",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "generic/:generic_identifier"
              ],
              "variable": [
                {
                  "id": "generic_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a generic publication."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "060d1f02-2a68-47ce-a0d3-092ff337ec61"
            }
          ]
        },
        {
          "id": "742f18c8-7a3a-467f-a8f1-a1ba321388bf",
          "name": "get-json-which-represents-the-structure-of-an-image",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "image/:image_identifier"
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
                  "id": "image_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an image."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b41c8960-6520-415c-b556-13d31f48e299"
            }
          ]
        },
        {
          "id": "20580876-694e-4ba2-a05b-a4179b399611",
          "name": "get-json-which-represents-the-structure-of-an-instrument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "instrument/:instrument_identifier"
              ],
              "variable": [
                {
                  "id": "instrument_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an instrument."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee49d235-a8f5-4262-8849-5d76305ae175"
            }
          ]
        },
        {
          "id": "deb55517-2f9c-4d8f-b89a-dad25790ed57",
          "name": "get-json-which-represents-the-structure-of-a-journal",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "journal/:journal_identifier"
              ],
              "variable": [
                {
                  "id": "journal_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a journal."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8cfc9f8-907a-4e43-9be0-0231fc5d2531"
            }
          ]
        },
        {
          "id": "53a3540c-4bd2-461e-bc4f-08ca3f306c2b",
          "name": "get-json-which-represents-the-structure-of-a-lexicon",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "lexicon/:lexicon_identifier"
              ],
              "variable": [
                {
                  "id": "lexicon_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a lexicon."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0ef3cfc-1247-48ec-9870-5af4bd2efe71"
            }
          ]
        },
        {
          "id": "bccc47e9-f952-4564-a920-1d5d96674a77",
          "name": "get-json-which-represents-the-structure-of-a-model",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "model/:model_identifier"
              ],
              "variable": [
                {
                  "id": "model_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a model."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0158f12-a5a0-4654-a638-da00e2af9a63"
            }
          ]
        },
        {
          "id": "689a1de7-6471-4ebd-9cac-bc2f47272848",
          "name": "get-json-which-represents-the-structure-of-a-model-run",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "model_run/:model_identifier/:scenario_identifier/:range_start/:range_end/:spatial_resolution/:time_resolution/:sequence"
              ],
              "variable": [
                {
                  "id": "model_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "range_end",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "range_start",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "scenario_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sequence",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "spatial_resolution",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "time_resolution",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a model run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0896abfd-7b30-4899-953f-6d42d48106a7"
            }
          ]
        },
        {
          "id": "383c0929-6d13-4308-b3b1-92223793287d",
          "name": "get-json-which-represents-the-structure-of-a-model-run",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "model_run/:model_run_identifier"
              ],
              "variable": [
                {
                  "id": "model_run_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a model run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95daf02d-e0db-4a16-9ec0-6e2a3bcf75b4"
            }
          ]
        },
        {
          "id": "f9993388-bd51-4839-9923-2586fcd235d6",
          "name": "get-json-which-represents-the-structure-of-an-organization",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "organization/:organization_identifier"
              ],
              "variable": [
                {
                  "id": "organization_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f0332b2-3f92-4be8-9d19-1b51233d880e"
            }
          ]
        },
        {
          "id": "f2dd869d-1092-419e-9aa8-d58635ad4931",
          "name": "get-json-which-represents-the-structure-of-a-person",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:person_identifier"
              ],
              "variable": [
                {
                  "id": "person_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a person."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cc43725-b5b1-4fda-83c1-7843953174b0"
            }
          ]
        },
        {
          "id": "4aeb533c-402b-403e-9bad-3563cdc5b22a",
          "name": "get-json-which-represents-the-structure-of-a-platform",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "platform/:platform_identifier"
              ],
              "variable": [
                {
                  "id": "platform_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a platform."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "580b6d7e-5f68-4751-bfc2-e519f6d27b9a"
            }
          ]
        },
        {
          "id": "9510c675-30ac-4bf0-9356-ecf1e3b03b5c",
          "name": "get-json-which-represents-the-structure-of-an-instrument-on-a-platform",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "platform/:platform_identifier/instrument/:instrument_identifier"
              ],
              "variable": [
                {
                  "id": "instrument_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "platform_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an instrument on a platform."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0694744f-2798-4a8b-9fd6-536a2deefd37"
            }
          ]
        },
        {
          "id": "f5f9801d-f9ca-429b-abc2-db5f5a48dad1",
          "name": "get-json-which-represents-the-structure-of-a-project",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "project/:project_identifier"
              ],
              "variable": [
                {
                  "id": "project_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acd76a99-abe2-4543-abb6-7a2692e579a7"
            }
          ]
        },
        {
          "id": "f8bd1ecb-38e4-4a82-ae5f-a0f689698a03",
          "name": "get-json-which-represents-the-structure-of-a-reference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "reference/:reference_identifier"
              ],
              "variable": [
                {
                  "id": "reference_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a reference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "313068f0-dd95-4e23-8ef3-5ba30670ce4e"
            }
          ]
        },
        {
          "id": "4505d258-e88b-4a92-b47a-fab17dbe7ace",
          "name": "get-json-which-represents-the-structure-of-a-region",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "region/:region_identifier"
              ],
              "variable": [
                {
                  "id": "region_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcfc132e-7e83-4d35-ad05-960a18c9a7da"
            }
          ]
        },
        {
          "id": "95c19fbc-0f2a-4902-beff-b08d5596c060",
          "name": "get-json-which-represents-the-structure-of-a-report",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier"
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
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a report."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d1b7365-6919-4e69-94d0-38d8231f3f79"
            }
          ]
        },
        {
          "id": "0f888fcc-eeb5-40dd-955a-f7509e033892",
          "name": "get-json-which-represents-the-structure-of-a-chapter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter/:chapter_identifier"
              ],
              "query": [
                {
                  "key": "ids",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
                  "id": "chapter_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a chapter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5937a2a5-fd95-4bca-8cec-13ccd8cf83c7"
            }
          ]
        },
        {
          "id": "d6661a68-33ea-4265-96b2-9904930339e6",
          "name": "get-json-which-represents-the-structure-of-a-figure-in-a-chapter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter/:chapter_identifier/figure/:figure_identifier"
              ],
              "query": [
                {
                  "key": "ids",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
                  "id": "chapter_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "figure_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a figure in a chapter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5b739f5-b8d9-4436-8b4c-f597c47ffff9"
            }
          ]
        },
        {
          "id": "d4964ba1-b19c-4767-8883-8eb7f9951059",
          "name": "get-json-which-represents-the-structure-of-a-finding-in-a-chapter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter/:chapter_identifier/finding/:finding_identifier"
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
                  "id": "chapter_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "finding_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a finding in a chapter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "373179ad-640b-4ef9-a053-1cd80c10777c"
            }
          ]
        },
        {
          "id": "20d62e99-2d6f-42c3-bb05-9b4d354e0b28",
          "name": "get-json-which-represents-the-structure-of-a-table-in-a-chapter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter/:chapter_identifier/table/:table_identifier"
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
                  "id": "chapter_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "table_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a table in a chapter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1641d856-274d-4092-a511-2fb2b7c4f998"
            }
          ]
        }
      ]
    },
    {
      "name": "Arrays",
      "item": [
        {
          "id": "794a768c-7acf-48f6-8e26-3f71d4bf95cc",
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
              "id": "86632deb-0bf4-40a5-815e-1c1b85372d38"
            }
          ]
        },
        {
          "id": "a783b921-15b9-46c5-bc9a-02e55f95d96c",
          "name": "list-the-arrays-associated-with-a-report-20-per-page",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/array"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the arrays associated with a report, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af0b2c3d-e2e1-4ef1-a70b-7edd477addc5"
            }
          ]
        }
      ]
    },
    {
      "name": "Articles",
      "item": [
        {
          "id": "7f7461d6-86b1-4977-839d-848fd83b804d",
          "name": "list-the-articles-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/article?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the articles, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0623f1d7-2172-423c-bebd-0070a1b2945d"
            }
          ]
        }
      ]
    },
    {
      "name": "Books",
      "item": [
        {
          "id": "68f28ffd-40b3-44f3-9fd6-ea27fb0e562a",
          "name": "list-the-books-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/book?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the books, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a3cae68-15ab-4f85-b51e-a4f5bac486a1"
            }
          ]
        },
        {
          "id": "11e02415-6396-44d7-aeec-0fa267673811",
          "name": "list-the-books-associated-with-a-report-20-per-page",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/book"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the books associated with a report, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ce7dd8f-8efb-4bd4-9103-28bbacec12ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Redirect",
      "item": [
        {
          "id": "208852e1-20d0-4f68-b38a-20ef21bdd68a",
          "name": "given-a-numeric-id-redirect-to-the-full-uri-of-a-contributor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "contributor/:contributor_identifier"
              ],
              "variable": [
                {
                  "id": "contributor_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a numeric ID, redirect to the full URI of a contributor."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12c7e57b-6235-4067-8b12-4615f7a99152"
            }
          ]
        },
        {
          "id": "3ed1f626-a3d4-4742-acbd-456bb10ce2bf",
          "name": "given-a-name-case-sensitive-concatenated-by-dashes-redirect-if-there-is-a-single-match--the-first-an",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a name (case sensitive, concatenated by dashes), redirect if there is a single match.  The first and last names can be in either order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "841fc2fa-6a91-4a21-b566-9fc0d8bc49cd"
            }
          ]
        },
        {
          "id": "cf396e03-1053-4959-93d7-37215c6f3523",
          "name": "given-an-orcid-if-there-is-a-match-redirect-to-the-persons-uri",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:orcid"
              ],
              "variable": [
                {
                  "id": "orcid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an ORCID, if there is a match, redirect to the persons URI."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4667b6b-47d0-48d7-a6a3-e4e4b2193c9a"
            }
          ]
        },
        {
          "id": "874894c6-3f4b-48e1-9c1e-de1d5bec2f6d",
          "name": "given-a-numeric-id-redirect-to-the-full-uri-of-a-publication",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "publication/:publication_identifier"
              ],
              "variable": [
                {
                  "id": "publication_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a numeric ID, redirect to the full URI of a publication."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd4740c1-1401-4a84-9faf-d8cd5debc171"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "44af284b-6797-49e5-bfd6-2056898f3b12",
          "name": "list-the-datasets-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/dataset?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the datasets, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7773f7b-f1e5-4f41-b479-1ec444cd0899"
            }
          ]
        }
      ]
    },
    {
      "name": "Look",
      "item": [
        {
          "id": "b719f8aa-8530-49a4-931a-be98ed0ec98d",
          "name": "given-a-doi-return-a-redirect-to-the-gcis-dataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "dataset/lookup/:doi"
              ],
              "variable": [
                {
                  "id": "doi",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a DOI, return a redirect to the GCIS dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa68fc65-399e-4142-b619-694ed7e80bb0"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "c461be42-a484-471e-aca2-a7fdebab6274",
          "name": "list-all-the-figures-in-gcis",
          "request": {
            "url": "http://data.globalchange.gov/figure?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all the figures in GCIS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ec4dc58-ffea-4096-908b-0df1cc69bd92"
            }
          ]
        }
      ]
    },
    {
      "name": "GCMD",
      "item": [
        {
          "id": "4ff4960a-c7d6-4425-80f8-77b3621ee942",
          "name": "list-the-gcmd-keywords-in-the-gcis-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/gcmd_keyword?page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the GCMD keywords in the GCIS, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "342f007d-a894-4cf5-8a87-17c598a68b49"
            }
          ]
        }
      ]
    },
    {
      "name": "Generic",
      "item": [
        {
          "id": "53a79384-108a-4063-a739-b02f1dd279a1",
          "name": "list-the-generic-publications-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/generic?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the generic publications, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2edc45f5-d8cd-46ab-9e47-27fb5b2733fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "ed9a149a-c8c9-4ca1-a303-9872886206f1",
          "name": "list-the-images-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/image?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the images, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2b04ec8-d7df-47e3-87ae-82996d696de4"
            }
          ]
        }
      ]
    },
    {
      "name": "Instruments",
      "item": [
        {
          "id": "47318ba2-cb71-4316-b30a-3ee915ee6a4c",
          "name": "list-the-instruments-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/instrument?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the instruments, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0046fbc-6d44-47dc-bfa4-880ef17ea71f"
            }
          ]
        },
        {
          "id": "cd820df6-dcdc-4371-a00a-4b93a10a27f1",
          "name": "list-the-instruments-on-a-platform-20-per-page",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "platform/:platform_identifier/instrument"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "platform_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the instruments on a platform, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4e91b26-ab8d-4ca7-9ff8-aec35ad0584f"
            }
          ]
        }
      ]
    },
    {
      "name": "Journals",
      "item": [
        {
          "id": "78fae8fe-93ac-470e-9abd-38c02d066de2",
          "name": "list-the-journals-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/journal?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the journals, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1138c2b-a2c2-4861-8fd6-35abfc6a95a4"
            }
          ]
        }
      ]
    },
    {
      "name": "Lexicons",
      "item": [
        {
          "id": "8ca8827c-18a7-411a-9101-45db44c66339",
          "name": "list-the-lexicons-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/lexicon?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the lexicons, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13c2ea31-5c60-4bf2-beb4-723dda7f330e"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "f9d88b56-f9b3-4b85-8029-c669421e1957",
          "name": "given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "lexicon/:lexicon_identifier/find/:context/:term"
              ],
              "variable": [
                {
                  "id": "context",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lexicon_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "term",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a lexicon, term, and context, return a 303 redirect to a GCID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b18d683d-b831-495d-8147-f1ab7af4815e"
            }
          ]
        },
        {
          "id": "2d20dbec-54fc-44db-80f8-522dd2b422b4",
          "name": "given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "lexicon/:lexicon_identifier/:context/:term"
              ],
              "variable": [
                {
                  "id": "context",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lexicon_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "term",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a lexicon, term, and context, return a 303 redirect to a GCID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2bacf47-2ba0-498a-b19e-8d60788c974d"
            }
          ]
        }
      ]
    },
    {
      "name": "Terms",
      "item": [
        {
          "id": "81af01a1-708b-4cd0-a5a3-d04e5a96a6dc",
          "name": "list-the-terms-within-a-context-of-a-lexicon",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "lexicon/:lexicon_identifier/list/:context"
              ],
              "variable": [
                {
                  "id": "context",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lexicon_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the terms within a context of a lexicon"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80f86b5d-18c9-4633-96c2-f346af41bb75"
            }
          ]
        }
      ]
    },
    {
      "name": "Overall",
      "item": [
        {
          "id": "af8dc5fa-15aa-41e2-b293-e69d532ff523",
          "name": "get-overall-metrics-about-gcis-data",
          "request": {
            "url": "http://data.globalchange.gov/metrics",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get overall metrics about GCIS data"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2db7b382-5f20-4419-a422-56b78240be75"
            }
          ]
        }
      ]
    },
    {
      "name": "Models",
      "item": [
        {
          "id": "b24a7cf0-1214-4353-8f7c-aab45c6c572e",
          "name": "list-the-models-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/model?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the models, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23c41c27-a91c-4670-9104-f405c449579d"
            }
          ]
        }
      ]
    },
    {
      "name": "Model",
      "item": [
        {
          "id": "f3e2efd8-c7a9-48fa-8eab-831d0268043b",
          "name": "list-the-model-runs-for-a-particular-model-20-per-page",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "model/:model_identifier/run"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "model_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the model runs for a particular model, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "932e36f9-73f7-420b-b202-f60e9d5febe3"
            }
          ]
        },
        {
          "id": "d5cacff8-911f-430b-9d79-aca407e65ef6",
          "name": "list-the-model-runs-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/model_run?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the model runs, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "871584a2-10cb-4614-84b9-f163eb4ddd2e"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "52121f20-bb2e-4d37-a3b7-3cc28fb1e3ca",
          "name": "list-the-organizations-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/organization?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the organizations, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc30effd-fad5-42a6-9799-366e559a3934"
            }
          ]
        }
      ]
    },
    {
      "name": "Show",
      "item": [
        {
          "id": "8e68cc10-c538-431a-a1b1-5f5251eaf99f",
          "name": "given-a-resource-dataset-report-etc-and-a-role-editor-etc-and-an-identifier-for-an-organization-show",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "organization/:organization_identifier/contributions/:role_type_identifier/:resource"
              ],
              "variable": [
                {
                  "id": "organization_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resource",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_type_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a resource (dataset, report, etc.) and a role (editor, etc), and an identifier for an organization, show the resources to which the organization has contributed in that role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8607a20-de8d-4b01-a132-f17617cc7f70"
            }
          ]
        },
        {
          "id": "ce10be25-2280-4e19-bd7f-8bc1c2e840d6",
          "name": "given-a-resource-dataset-report-etc-and-a-role-editor-etc-and-an-identifier-for-a-person-show-the-re",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:person_identifier/contributions/:role_type_identifier/:resource"
              ],
              "variable": [
                {
                  "id": "person_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resource",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_type_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a resource (dataset, report, etc.) and a role (editor, etc), and an identifier for a person, show the resources to which the person has contributed in that role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "221bcc89-edb0-4608-8b8b-5901920052c8"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "a661c59e-0ed1-4e09-8d9d-f6100156f80b",
          "name": "list-the-people-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/person?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the people, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01dcabed-eb48-440e-86e9-0a5bc82ce125"
            }
          ]
        }
      ]
    },
    {
      "name": "Platforms",
      "item": [
        {
          "id": "8adae578-769e-4325-8205-796d77b338e9",
          "name": "list-the-platforms-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/platform?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the platforms, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a0de490-8611-499d-8021-9b8242a3e5b9"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "31789eac-acdf-4279-aefc-fd98655de23f",
          "name": "list-the-projects-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/project?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the projects, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05310475-fe02-40ab-aa4b-7097b2456a15"
            }
          ]
        }
      ]
    },
    {
      "name": "References",
      "item": [
        {
          "id": "391da9f8-263e-4840-b017-5aa93ae195df",
          "name": "list-the-references-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/reference?page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the references, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24a92509-1049-4842-ad0f-1ebb8a9d5cec"
            }
          ]
        },
        {
          "id": "05f9c799-438e-4aa9-9429-4aecffea42db",
          "name": "get-a-list-of-references-in-a-chapter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter/:chapter_identifier/reference"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "chapter_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of references in a chapter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f824025-6789-43d6-afdc-d5a6186f92b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "b8cb3e87-ea98-4107-ac36-40d03279e64f",
          "name": "list-the-regions-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/region?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the regions, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c81ea4d2-564b-48ed-beea-f02f0b4add13"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "66077621-c6ed-4a5d-a788-6ac63572ebe1",
          "name": "list-the-reports-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/report?all=%7B%7D&page=%7B%7D&report_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the reports, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74feb0ab-3116-4b20-a64d-75c02e926ad9"
            }
          ]
        }
      ]
    },
    {
      "name": "Chapters",
      "item": [
        {
          "id": "228a2b93-a5c6-4b9b-a681-7d54910d26ec",
          "name": "get-a-list-of-chapters-in-a-report",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of chapters in a report."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "046aff01-77e2-48e8-a7c6-11abb4fb328a"
            }
          ]
        }
      ]
    },
    {
      "name": "Figures",
      "item": [
        {
          "id": "5e3ee1d8-fdae-4135-80ee-0619bce75ec1",
          "name": "get-a-list-of-figures-in-a-chapter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter/:chapter_identifier/figure"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ids",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "chapter_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of figures in a chapter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "801ce216-9226-4f99-bd5b-26b292e14073"
            }
          ]
        },
        {
          "id": "67dc3e1f-95b4-482c-990e-6dd5cad05704",
          "name": "list-the-figures-in-a-report-20-per-page",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/figure"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the figures in a report, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c39f442-e6b5-453a-9578-381c548b9230"
            }
          ]
        }
      ]
    },
    {
      "name": "Findings",
      "item": [
        {
          "id": "191a97f2-2a8a-4b5e-8aaa-3b687362363d",
          "name": "get-a-list-of-findings-in-a-chapter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter/:chapter_identifier/finding"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ids",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "chapter_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of findings in a chapter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97eb867c-d98a-4046-bfce-fe4a490fa8ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Tables",
      "item": [
        {
          "id": "f09e75c8-2755-4306-96ec-2aba838f03bd",
          "name": "get-a-list-of-tables-in-a-chapter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "report/:report_identifier/chapter/:chapter_identifier/table"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "chapter_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of tables in a chapter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b44f7891-661b-4ca0-aa00-4cc0cf341e79"
            }
          ]
        }
      ]
    }
  ]
}