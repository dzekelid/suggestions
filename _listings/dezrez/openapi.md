swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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