---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 0
info:
  title: AWS CloudSearch Delete Suggester
  version: 1.0.0
  description: Deletes a suggester.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BuildSuggesters:
    get:
      summary: Build Suggesters
      description: Indexes the search suggestions.
      operationId: BuildSuggesters
      x-api-path-slug: actionbuildsuggesters-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
  /?Action=DefineSuggester:
    get:
      summary: Define Suggester
      description: Configures a suggester for a domain.
      operationId: DefineSuggester
      x-api-path-slug: actiondefinesuggester-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: Suggester
        description: Configuration information for a search suggester
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
  /?Action=DeleteSuggester:
    get:
      summary: Delete Suggester
      description: Deletes a suggester.
      operationId: DeleteSuggester
      x-api-path-slug: actiondeletesuggester-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: SuggesterName
        description: Specifies the name of the suggester you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
  /?Action=DescribeSuggesters:
    get:
      summary: Describe Suggesters
      description: Gets the suggesters configured for a domain.
      operationId: DescribeSuggesters
      x-api-path-slug: actiondescribesuggesters-get
      parameters:
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      - in: query
        name: SuggesterNames.member.N
        description: The suggesters you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
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