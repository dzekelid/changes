---
swagger: "2.0"
info:
  title: Intrinio API Exchange Prices
  description: Returns professional-grade historical stock prices for all securities
    traded on a stock exchange for a single specified day.  Historical prices are
    available back to 1996 or the IPO date, with some companies with data back to
    the 1970s.
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /prices/exchange:
    get:
      summary: Exchange Prices
      description: Returns professional-grade historical stock prices for all securities
        traded on a stock exchange for a single specified day
      operationId: exchange-prices
      parameters:
      - in: query
        name: identifier
        description: ' the stock market ticker symbol associated with the companies
          common stock securities or the stock market index: '
        type: string
      - in: query
        name: page_number
        description: ' an integer greater than or equal to 1 for specifying the page
          number for the return values'
        type: string
      - in: query
        name: page_size
        description: ' an integer greater than 1 for specifying the number of results
          on each page'
        type: string
      - in: query
        name: price_date
        description: ' the specified date in which historical stock prices are returned
          for a stock exchange '
        type: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - prices
      - exchanges
definitions: []
x-collection-name: Intrinio
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