---
swagger: "2.0"
x-collection-name: Europeana
x-complete: 0
info:
  title: Europeana get autocompletion recommendations for search queries
  description: Get autocompletion recommendations for search queries.
  termsOfService: http://www.europeana.eu/portal/en/rights.html
  contact:
    name: http://labs.europeana.eu/api
  version: 1.0.0
host: www.europeana.eu
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /suggestions.json:
    get:
      summary: get autocompletion recommendations for search queries
      description: Get autocompletion recommendations for search queries.
      operationId: suggestions
      x-api-path-slug: suggestions-json-get
      parameters:
      - in: query
        name: callback
        description: callback
      - in: query
        name: phrases
        description: phrases
      - in: query
        name: query
        description: query
      - in: query
        name: rows
        description: rows
      responses:
        200:
          description: OK
      tags:
      - Suggestions
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