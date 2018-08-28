swagger: "2.0"
x-collection-name: Europeana
x-complete: 1
info:
  title: Europeana
  description: this-swagger-api-console-provides-an-overview-of-an-interface-to-the-europeana-rest-api--you-can-build-and-test-anything-from-the-simplest-search-to-a-complex-query-using-facetlist-such-as-dates-geotags-and-permissions--for-more-help-and-information-head-to-our-comprehensive-a-hrefhttplabs-europeana-euapionline-documentationa-
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