---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API List articles.
  description: List the articles, 20 per page.
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activity:
    get:
      summary: List activities.
      description: List the activities, 20 per page.
      operationId: list-the-activities-20-per-page
      x-api-path-slug: activity-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the activities
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Activities
  /activity/{activity_identifier}:
    get:
      summary: Get a representation of an activity.
      description: Get JSON which represents the structure of an activity.
      operationId: get-json-which-represents-the-structure-of-an-activity
      x-api-path-slug: activityactivity-identifier-get
      parameters:
      - in: path
        name: activity_identifier
        description: activity_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Activity
  /array:
    get:
      summary: List arrays.
      description: List the arrays, 20 per page.
      operationId: list-the-arrays-20-per-page
      x-api-path-slug: array-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the arrays
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Arrays
  /array/{array_identifier}:
    get:
      summary: Get a representation of an array.
      description: Get JSON which represents the structure of an array.
      operationId: get-json-which-represents-the-structure-of-an-array
      x-api-path-slug: arrayarray-identifier-get
      parameters:
      - in: path
        name: array_identifier
        description: array_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the array
      - in: query
        name: with_regions
        description: Include regions associated with the array
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Array
  /article:
    get:
      summary: List articles.
      description: List the articles, 20 per page.
      operationId: list-the-articles-20-per-page
      x-api-path-slug: article-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the articles
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Articles
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---