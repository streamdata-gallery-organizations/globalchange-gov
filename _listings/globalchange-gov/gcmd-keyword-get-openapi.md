---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API List GCMD keywords in the GCIS.
  description: List the GCMD keywords in the GCIS, 20 per page.
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
  /article/{article_identifier}:
    get:
      summary: Get a representation of an article.
      description: Get JSON which represents the structure of an article.
      operationId: get-json-which-represents-the-structure-of-an-article
      x-api-path-slug: articlearticle-identifier-get
      parameters:
      - in: path
        name: article_identifier
        description: article_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the article
      - in: query
        name: with_regions
        description: Include regions associated with the article
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Article
  /book:
    get:
      summary: List books.
      description: List the books, 20 per page.
      operationId: list-the-books-20-per-page
      x-api-path-slug: book-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the books
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Books
  /book/{book_identifier}:
    get:
      summary: Get a representation of a book.
      description: Get JSON which represents the structure of a book.
      operationId: get-json-which-represents-the-structure-of-a-book
      x-api-path-slug: bookbook-identifier-get
      parameters:
      - in: path
        name: book_identifier
        description: book_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the book
      - in: query
        name: with_regions
        description: Include regions associated with the book
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Book
  /contributor/{contributor_identifier}:
    get:
      summary: Redirect to a particular contributor.
      description: Given a numeric ID, redirect to the full URI of a contributor.
      operationId: given-a-numeric-id-redirect-to-the-full-uri-of-a-contributor
      x-api-path-slug: contributorcontributor-identifier-get
      parameters:
      - in: path
        name: contributor_identifier
        description: contributor_identifier description
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - To
      - Particular
      - Contributor
  /dataset:
    get:
      summary: List datasets.
      description: List the datasets, 20 per page.
      operationId: list-the-datasets-20-per-page
      x-api-path-slug: dataset-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the datasets
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /dataset/lookup/{doi}:
    get:
      summary: Look up a dataset by DOI.
      description: Given a DOI, return a redirect to the GCIS dataset.
      operationId: given-a-doi-return-a-redirect-to-the-gcis-dataset
      x-api-path-slug: datasetlookupdoi-get
      parameters:
      - in: path
        name: doi
        description: doi description
      responses:
        200:
          description: OK
      tags:
      - Look
      - Up
      - Dataset
      - By
      - DOI
  /dataset/{dataset_identifier}:
    get:
      summary: Get a representation of a dataset.
      description: Get JSON which represents the structure of a dataset.
      operationId: get-json-which-represents-the-structure-of-a-dataset
      x-api-path-slug: datasetdataset-identifier-get
      parameters:
      - in: path
        name: dataset_identifier
        description: dataset_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Dataset
  /figure:
    get:
      summary: List all figures
      description: List all the figures in GCIS.
      operationId: list-all-the-figures-in-gcis
      x-api-path-slug: figure-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the figures
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - ""
      - Figures
  /file/{file_identifier}:
    get:
      summary: Get a representation of a file.
      description: Get JSON which represents the structure of a file.
      operationId: get-json-which-represents-the-structure-of-a-file
      x-api-path-slug: filefile-identifier-get
      parameters:
      - in: path
        name: file_identifier
        description: file_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - File
  /gcmd_keyword:
    get:
      summary: List GCMD keywords in the GCIS.
      description: List the GCMD keywords in the GCIS, 20 per page.
      operationId: list-the-gcmd-keywords-in-the-gcis-20-per-page
      x-api-path-slug: gcmd-keyword-get
      parameters:
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - GCMD
      - Keywords
      - GCIS
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