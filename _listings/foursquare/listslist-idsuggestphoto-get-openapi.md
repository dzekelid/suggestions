---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Lists Suggestphoto
  description: /lists/{LIST_ID}/followers
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{LIST_ID}/suggestphoto:
    get:
      summary: Get Lists Suggestphoto
      description: /lists/{LIST_ID}/followers
      operationId: listslist-idfollowers
      x-api-path-slug: listslist-idsuggestphoto-get
      parameters:
      - in: query
        name: itemId
        description: Id of item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggestphoto
  /lists/{LIST_ID}/suggesttip:
    get:
      summary: Get Lists Suggesttip
      description: /lists/{LIST_ID}/suggestphoto
      operationId: listslist-idsuggestphoto
      x-api-path-slug: listslist-idsuggesttip-get
      parameters:
      - in: query
        name: itemId
        description: Id of item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggesttip
  /venues/suggestcompletion:
    get:
      summary: Get Venues Suggestcompletion
      description: /venues/search
      operationId: venuessearch
      x-api-path-slug: venuessuggestcompletion-get
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Accuracy of the users altitude, in meters
      - in: query
        name: limit
        description: Number of results to return, up to 100
      - in: query
        name: ll
        description: Latitude and longitude of the users location
      - in: query
        name: llAcc
        description: Accuracy of latitude and longitude, in meters
      - in: query
        name: query
        description: A search term to be applied against titles
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Suggestcompletion
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