---
name: Intrinio
x-slug: intrinio
description: Market for financial data APIs and analytics applications built with
  those data feeds. Affordable, easy to access financial data for developers and investors
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
x-kinRank: "8"
x-alexaRank: "321628"
tags: Changes
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/intrinio/apis.md
specificationVersion: "0.14"
apis:
- name: Intrinio API Stock Exchange Master
  x-api-slug: intrinio-api
  description: Returns stock exchange list and information for all stock exchanges
    covered by Intrinio.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com////stock_exchanges
  tags: Market Data,Stock Exchanges
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/intrinio/stock-exchanges-get-openapi.md
- name: Intrinio API Exchange Prices
  x-api-slug: intrinio-api
  description: Returns professional-grade historical stock prices for all securities
    traded on a stock exchange for a single specified day.  Historical prices are
    available back to 1996 or the IPO date, with some companies with data back to
    the 1970s.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com////prices/exchange
  tags: Market Data,Prices,Exchanges
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/intrinio/pricesexchange-get-openapi.md
- name: Intrinio API Stock Exchange Corporate Actions
  x-api-slug: intrinio-api
  description: 'Returns all corporate actions for all securities listed on a specified
    stock exchange.  A subscription to the EDI Corporate Actions Data Feed for a specific
    country will permit access to all stock exchanges in that country (ie, US includes
    NASDAQ, NYSE, BATS). Events 45+ types of corporate actions such as: Announcements
    and Annual Shareholder Meetings, Ex-date, Dividend pay date, Splits, Buy Backs,
    M&amp;A and Takeovers, Bankruptcies and much more'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com////stock_exchanges/corporate_actions
  tags: Market Data,Stock Exchanges
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/intrinio/stock-exchangescorporate-actions-get-openapi.md
- name: Intrinio API
  x-api-slug: intrinio-api
  description: Market for financial data APIs and analytics applications built with
    those data feeds. Affordable, easy to access financial data for developers and
    investors
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com//
  tags: Changes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/intrinio/openapi.md
x-common:
- type: x-applications-showcase
  url: https://intrinio.com/marketplace/apps
- type: x-authentication
  url: http://docs.intrinio.com/#authentication
- type: x-blog
  url: http://blog.intrinio.com/
- type: x-blog-rss
  url: http://blog.intrinio.com/feed/
- type: x-code
  url: http://docs.intrinio.com/#sdks
- type: x-crunchbase
  url: https://crunchbase.com/organization/tribunat
- type: x-developer
  url: https://intrinio.com/we-love-developers
- type: x-documentation
  url: https://intrinio.com/marketplace/data
- type: x-email
  url: cfarley@intrinio.com
- type: x-email
  url: admin@intrinio.com
- type: x-email
  url: support@intrinio.com
- type: x-login
  url: https://intrinio.com/login
- type: x-partners
  url: https://intrinio.com/partners
- type: x-press
  url: https://intrinio.com/press
- type: x-rate-limits
  url: http://docs.intrinio.com/#limits
- type: x-selfservice-registration
  url: https://intrinio.com/signup
- type: x-spreadsheets
  url: http://docs.intrinio.com/#spreadsheet-add-ins
- type: x-support
  url: https://intrinio.com/help
- type: x-tutorial
  url: https://intrinio.com/tutorial/web_api
- type: x-twitter
  url: https://twitter.com/intrinio
- type: x-website
  url: https://intrinio.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---