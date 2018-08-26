---
swagger: "2.0"
x-collection-name: TradeStation
x-complete: 0
info:
  title: TradeStation Stream Quote Changes
  description: |-
    Streams the latest Quote information for the given Symbols. The first chunk in the stream is a full quote snapshot - subsequent chunks only contain fields of the quote object that have changed since the last chunk.

    An invalid symbol name will result in a response of this form - {"Symbol":"BADEXAMPLESYMBOL","Error":"FAILED, EX_INVALID_SYMBOL"}

    If the user is not entitled for the symbol requested, response will be of this form - {"Symbol":"EXAMPLESYMBOL","Error":"FAILED, EX_NOT_ENTITLED"}
  termsOfService: http://elasticbeanstalk-us-east-1-525856068889.s3.amazonaws.com/wp-content/uploads/2014/03/Guidelines_For_Acceptance.pdf
  contact:
    name: TradeStation API Team
    url: https://developer.tradestation.com/webapi
    email: webapi@tradestation.com
  version: 1.0.0
host: api.tradestation.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stream/quote/changes/{symbols}:
    get:
      summary: Stream Quote Changes
      description: |-
        Streams the latest Quote information for the given Symbols. The first chunk in the stream is a full quote snapshot - subsequent chunks only contain fields of the quote object that have changed since the last chunk.

        An invalid symbol name will result in a response of this form - {"Symbol":"BADEXAMPLESYMBOL","Error":"FAILED, EX_INVALID_SYMBOL"}

        If the user is not entitled for the symbol requested, response will be of this form - {"Symbol":"EXAMPLESYMBOL","Error":"FAILED, EX_NOT_ENTITLED"}
      operationId: streamQuotesChanges
      x-api-path-slug: streamquotechangessymbols-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbols
        description: 1 or more Symbol Names (comma-separated)
      - in: header
        name: Transfer-Encoding
        description: a header with the value of `Chunked` must be passed to streaming
          resources
      responses:
        200:
          description: Successful response
      tags:
      - Stream
      - Quote
      - Changes
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