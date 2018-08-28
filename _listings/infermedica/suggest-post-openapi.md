---
swagger: "2.0"
x-collection-name: Infermedica
x-complete: 0
info:
  title: Infermedica Post Suggest
  description: Suggests possible symptoms based on provided patient information.
  version: v2
host: api.infermedica.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /suggest:
    post:
      summary: Post Suggest
      description: Suggests possible symptoms based on provided patient information.
      operationId: postSuggest
      x-api-path-slug: suggest-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: max_results
        description: maximum number of results
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Suggest
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