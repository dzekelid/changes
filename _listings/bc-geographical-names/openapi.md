---
swagger: "2.0"
x-collection-name: BC Geographical Names
x-complete: 1
info:
  title: BC Geographical Names
  description: this-rest-api-provides-searchable-access-to-information-about-geographical-names-in-the-province-of-british-columbia-including-name-status-and-details-about-the-corresponding-geographic-feature-
  contact:
    name: BC Geographical Names Office
    email: geographical.names@gov.bc.ca
  version: 3.x.x
host: apps.gov.bc.ca
basePath: /pub/bcgnws
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /names/changes:
    get:
      summary: Search for names with metadata changes in a given period
      description: Search for information about geographical names which have changed
        most recently within a specified time window.  Changes may include status
        cupdates and metadata corrections.
      operationId: search-for-information-about-geographical-names-which-have-changed-most-recently-within-a-specified-
      x-api-path-slug: nameschanges-get
      parameters:
      - in: query
        name: embed
        description: A flag to indicate whether to embed the corresponding feature
          into each matching name
      - in: query
        name: featureCategory
        description: A filter to limit the search to names associated with features
          of a certain category  The value of this parameter should be a featureCategoryCode
          value returned by the /featureCategories resource, or an asterisk (*) to
          request that all feature categories be included
      - in: query
        name: featureClass
        description: A filter to limit the search to names associated with features
          of a certain class  The value of this parameter should be a featureClassCode
          value returned by the /featureClasses resource, or an asterisk (*) to request
          that all feature classes be included
      - in: query
        name: featureType
        description: A filter to limit the search to names associated with features
          of a certain type  The value of this parameter should be a featureTypeCode
          value returned by the /featureTypes resource, or an asterisk (*) to request
          that all feature types be included
      - in: query
        name: fromDate
        description: Defines the earliest date (YYYY-MM-DD format) of the change time
          window for the search
      - in: query
        name: itemsPerPage
        description: The number of search results to return (1-200)
      - in: query
        name: outputFormat
        description: The format of the output
      - in: query
        name: outputSRS
        description: The EPSG code of the spatial reference system (SRS) to use for
          output geometries
      - in: query
        name: outputStyle
        description: A flag indicating whether to include with each matching name
          a succinct list of attributes (summary), or a comprehensive list of attributes
          (detail)
      - in: query
        name: sortBy
        description: The distance to move the accessPoint away from the curb and towards
          the inside of the parcel (in metres)
      - in: query
        name: startIndex
        description: The index of the first record to be returned (>= 1)
      - in: query
        name: toDate
        description: Defines the latest date (YYYY-MM-DD format) of the change time
          window for the search
      responses:
        200:
          description: OK
      tags:
      - Names
      - Changes
---