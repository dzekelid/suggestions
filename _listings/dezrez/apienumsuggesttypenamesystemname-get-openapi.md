---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get enum suggestions for value
  version: 1.0.0
  description: Get enum suggestions for value.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/enum/suggest/{typeName}/{systemName}:
    get:
      summary: Get enum suggestions for value
      description: Get enum suggestions for value.
      operationId: Enum_SuggestBytypeNameBysystemName
      x-api-path-slug: apienumsuggesttypenamesystemname-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: systemName
        description: The value to retrieve suggestions for
      - in: path
        name: typeName
        description: The type of enum to get
      responses:
        200:
          description: OK
      tags:
      - Enum
      - Suggestionsvalue
  /api/feature/suggest:
    get:
      summary: Get feature suggestions for value
      description: Get feature suggestions for value.
      operationId: Feature_SuggestByname
      x-api-path-slug: apifeaturesuggest-get
      parameters:
      - in: query
        name: name
        description: The value to retrieve suggestions for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Feature
      - Suggestionsvalue
  /api/tag/suggest:
    get:
      summary: Get tag suggestions for value
      description: Get tag suggestions for value.
      operationId: Tag_SuggestByname
      x-api-path-slug: apitagsuggest-get
      parameters:
      - in: query
        name: name
        description: The value to retrieve suggestions for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Suggestionsvalue
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