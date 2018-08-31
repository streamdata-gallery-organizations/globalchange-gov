---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Lookup a GCID from a term
  description: Given a lexicon, term, and context, return a 303 redirect to a GCID
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
  /gcmd_keyword/{gcmd_keyword_identifier}:
    get:
      summary: Get a representation of a GCMD keyword.
      description: Get JSON which represents the structure of a GCMD keyword.
      operationId: get-json-which-represents-the-structure-of-a-gcmd-keyword
      x-api-path-slug: gcmd-keywordgcmd-keyword-identifier-get
      parameters:
      - in: path
        name: gcmd_keyword_identifier
        description: gcmd_keyword_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - GCMD
      - Keyword
  /generic:
    get:
      summary: List generic publications.
      description: List the generic publications, 20 per page.
      operationId: list-the-generic-publications-20-per-page
      x-api-path-slug: generic-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the generic publications
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Generic
      - Publications
  /generic/{generic_identifier}:
    get:
      summary: Get a representation of a generic publication.
      description: Get JSON which represents the structure of a generic publication.
      operationId: get-json-which-represents-the-structure-of-a-generic-publication
      x-api-path-slug: genericgeneric-identifier-get
      parameters:
      - in: path
        name: generic_identifier
        description: generic_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Generic
      - Publication
  /image:
    get:
      summary: List images.
      description: List the images, 20 per page.
      operationId: list-the-images-20-per-page
      x-api-path-slug: image-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the images
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Images
  /image/{image_identifier}:
    get:
      summary: Get a representation of an image.
      description: Get JSON which represents the structure of an image.
      operationId: get-json-which-represents-the-structure-of-an-image
      x-api-path-slug: imageimage-identifier-get
      parameters:
      - in: path
        name: image_identifier
        description: image_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the image
      - in: query
        name: with_regions
        description: Include regions associated with the image
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Image
  /instrument:
    get:
      summary: List instruments.
      description: List the instruments, 20 per page.
      operationId: list-the-instruments-20-per-page
      x-api-path-slug: instrument-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the instruments
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Instruments
  /instrument/{instrument_identifier}:
    get:
      summary: Get a representation of an instrument.
      description: Get JSON which represents the structure of an instrument.
      operationId: get-json-which-represents-the-structure-of-an-instrument
      x-api-path-slug: instrumentinstrument-identifier-get
      parameters:
      - in: path
        name: instrument_identifier
        description: instrument_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Instrument
  /journal:
    get:
      summary: List journals.
      description: List the journals, 20 per page.
      operationId: list-the-journals-20-per-page
      x-api-path-slug: journal-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the journals
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Journals
  /journal/{journal_identifier}:
    get:
      summary: Get a representation of a journal.
      description: Get JSON which represents the structure of a journal.
      operationId: get-json-which-represents-the-structure-of-a-journal
      x-api-path-slug: journaljournal-identifier-get
      parameters:
      - in: path
        name: journal_identifier
        description: journal_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Journal
  /lexicon:
    get:
      summary: List lexicons.
      description: List the lexicons, 20 per page.
      operationId: list-the-lexicons-20-per-page
      x-api-path-slug: lexicon-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the lexicons
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Lexicons
  /lexicon/{lexicon_identifier}:
    get:
      summary: Get a representation of a lexicon.
      description: Get JSON which represents the structure of a lexicon.
      operationId: get-json-which-represents-the-structure-of-a-lexicon
      x-api-path-slug: lexiconlexicon-identifier-get
      parameters:
      - in: path
        name: lexicon_identifier
        description: lexicon_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Lexicon
  /lexicon/{lexicon_identifier}/find/{context}/{term}:
    get:
      summary: Lookup a GCID from a term
      description: Given a lexicon, term, and context, return a 303 redirect to a
        GCID
      operationId: given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid
      x-api-path-slug: lexiconlexicon-identifierfindcontextterm-get
      parameters:
      - in: path
        name: context
        description: context description
      - in: path
        name: lexicon_identifier
        description: lexicon_identifier description
      - in: path
        name: term
        description: term description
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - GCID
      - From
      - Term
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