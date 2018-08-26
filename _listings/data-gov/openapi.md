---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datasets/suggest/:
    get:
      summary: Get Datasets Suggest
      description: Suggest datasets
      operationId: getDatasetsSuggest
      x-api-path-slug: datasetssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Suggest
  /datasets/suggest/formats/:
    get:
      summary: Get Datasets Suggest Formats
      description: Suggest file formats
      operationId: getDatasetsSuggestFormats
      x-api-path-slug: datasetssuggestformats-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Suggest
      - Formats
  /organizations/suggest/:
    get:
      summary: Get Organizations Suggest
      description: Suggest organizations
      operationId: getOrganizationsSuggest
      x-api-path-slug: organizationssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Suggest
  /reuses/suggest/:
    get:
      summary: Get Reuses Suggest
      description: Suggest reuses
      operationId: getReusesSuggest
      x-api-path-slug: reusessuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Suggest
  /spatial/zones/suggest:
    get:
      summary: Get Spatial Zones Suggest
      description: Suggest geospatial zones
      operationId: getSpatialZonesSuggest
      x-api-path-slug: spatialzonessuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Zones
      - Suggest
  /tags/suggest/:
    get:
      summary: Get Tags Suggest
      description: Suggest tags
      operationId: getTagsSuggest
      x-api-path-slug: tagssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Suggest
  /territory/suggest/:
    get:
      summary: Get Territory Suggest
      description: ""
      operationId: getTerritorySuggest
      x-api-path-slug: territorysuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The maximum result size
      responses:
        200:
          description: OK
      tags:
      - Territory
      - Suggest
  /users/suggest/:
    get:
      summary: Get Users Suggest
      description: Suggest users
      operationId: getUsersSuggest
      x-api-path-slug: userssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Users
      - Suggest
---