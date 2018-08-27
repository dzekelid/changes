---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Returns list of unique ShowId changes greater than
    or equal to date (UTC).
  description: All new and updated shows from requested date and time.  When a record
    gets updated, use the ID to get the full show object and replace the data in your
    cache.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Changes/Episodes/History/:
    get:
      summary: Returns list of unique EpisodeId changes greater than or equal to date
        (UTC)
      description: For each updated episode ID, pull the full episode data for that
        ID and update.
      operationId: GetEpisodeChangeHistory
      x-api-path-slug: changesepisodeshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Episodes
      - History
  /Changes/Episodes/HistoryWithEntity/:
    get:
      summary: Returns list of unique EpisodeId and Entity changes greater than or
        equal to date (UTC).
      description: Lists each episode ID that has changed as well as the entity in
        the object that changed.
      operationId: GetEpisodeChangeHistoryWithEntity
      x-api-path-slug: changesepisodeshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Episodes
      - HistoryWithEntity
  /Changes/Movies/History/:
    get:
      summary: Returns list of unique MovieId changes greater than or equal to date
        (UTC).
      description: Use to get the ID's of the movies that have been added or changed
        and use /Movies/{ID} to get back the object with the updated data and replace
        in your database.
      operationId: GetMovieChangeHistory
      x-api-path-slug: changesmovieshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Movies
      - History
  /Changes/Movies/HistoryWithEntity/:
    get:
      summary: Returns list of unique MovieId and Entity changes greater than or equal
        to date (UTC).
      description: Same as /Changes/Movies/History but with the specific entities
        that have changed inside the MovieResponse.
      operationId: GetMovieChangeHistoryWithEntity
      x-api-path-slug: changesmovieshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Movies
      - HistoryWithEntity
  /Changes/People/History/:
    get:
      summary: Returns list of unique PersonId changes greater than or equal to date
        (UTC).
      description: Requires a valid Date.
      operationId: GetPersonChangeHistory
      x-api-path-slug: changespeoplehistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - People
      - History
  /Changes/People/HistoryWithEntity/:
    get:
      summary: Returns list of unique PersonId and Entity changes greater than or
        equal to date (UTC).
      description: Requires a valid Date.
      operationId: GetPersonChangeHistoryWithEntity
      x-api-path-slug: changespeoplehistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - People
      - HistoryWithEntity
  /Changes/Seasons/History/:
    get:
      summary: Returns list of unique SeasonId changes greater than or equal to date
        (UTC).
      description: Use if you want to check for specific updates to season records.
      operationId: GetSeasonChangeHistory
      x-api-path-slug: changesseasonshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Seasons
      - History
  /Changes/Seasons/HistoryWithEntity/:
    get:
      summary: Returns list of unique SeasonId and Entity changes greater than or
        equal to date (UTC).
      description: Returns list of new or changed SeasonIds with the entity that has
        changed.
      operationId: GetSeasonChangeHistoryWithEntity
      x-api-path-slug: changesseasonshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Seasons
      - HistoryWithEntity
  /Changes/Shows/History/:
    get:
      summary: Returns list of unique ShowId changes greater than or equal to date
        (UTC).
      description: All new and updated shows from requested date and time.  When a
        record gets updated, use the ID to get the full show object and replace the
        data in your cache.
      operationId: GetShowChangeHistory
      x-api-path-slug: changesshowshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Shows
      - History
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