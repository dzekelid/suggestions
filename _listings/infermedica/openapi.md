---
swagger: "2.0"
x-collection-name: Infermedica
x-complete: 1
info:
  title: Infermedica
  description: empower-your-healthcare-services-with-intelligent-diagnostic-insights-of-infermedica-api-
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
---