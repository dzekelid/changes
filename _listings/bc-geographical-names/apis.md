---
name: BC Geographical Names
x-slug: bc-geographical-names
description: Geographical names are more than labels on maps and road signs. They
  can reveal patterns of settlement, exploration and migration, and mirror outside
  influences to our history - aspects of the heritage and promise of an area that
  might otherwise be overlooked or forgotten by visitors and later generations.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Changes
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/bc-geographical-names/apis.md
specificationVersion: "0.14"
apis:
- name: BC Geographical Names Search for names with metadata changes in a given period
  x-api-slug: bc-geographical-names
  description: Search for information about geographical names which have changed
    most recently within a specified time window.  Changes may include status cupdates
    and metadata corrections.
  image: ""
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/bcgnws//names/changes
  tags: Names,Changes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/bc-geographical-names/nameschanges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/bc-geographical-names/nameschanges-get-openapi.md
- name: BC Geographical Names
  x-api-slug: bc-geographical-names
  description: Geographical names are more than labels on maps and road signs. They
    can reveal patterns of settlement, exploration and migration, and mirror outside
    influences to our history - aspects of the heritage and promise of an area that
    might otherwise be overlooked or forgotten by visitors and later generations.
  image: ""
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/bcgnws
  tags: Changes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/bc-geographical-names/openapi.md
x-common:
- type: x-website
  url: https://apps.gov.bc.ca/pub/bcgnws/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---