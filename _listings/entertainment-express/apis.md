---
name: Entertainment Express
x-slug: entertainment-express
description: Internet Video Archive (IVA) is a leading entertainment data company
  providing metadata, images and trailers/clips, for movie and TV content. With the
  launch of its award-winning Entertainment Express APIs, clients can easily access
  everything they need to create engaging content discovery experiences. By using
  Entertainment Express, clients can also connect to other services like movie showtimes
  and ticketing, content recommendations, content availability and TV channel line-ups.
  With over a million titles, episodes and over 150,000 videos available, IVA makes
  it easy for developers to integrate all the services they need at a very affordable
  price.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Changes
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/apis.md
specificationVersion: "0.14"
apis:
- name: Entertainment Express - Returns list of unique EpisodeId changes greater than
    or equal to date (UTC)
  x-api-slug: changesepisodeshistory-get
  description: For each updated episode ID, pull the full episode data for that ID
    and update.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesepisodeshistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesepisodeshistory-get-openapi.md
- name: Entertainment Express - Returns list of unique EpisodeId and Entity changes
    greater than or equal to date (UTC).
  x-api-slug: changesepisodeshistorywithentity-get
  description: Lists each episode ID that has changed as well as the entity in the
    object that changed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesepisodeshistorywithentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesepisodeshistorywithentity-get-openapi.md
- name: Entertainment Express - Returns list of unique MovieId changes greater than
    or equal to date (UTC).
  x-api-slug: changesmovieshistory-get
  description: Use to get the ID's of the movies that have been added or changed and
    use /Movies/{ID} to get back the object with the updated data and replace in your
    database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesmovieshistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesmovieshistory-get-openapi.md
- name: Entertainment Express - Returns list of unique MovieId and Entity changes
    greater than or equal to date (UTC).
  x-api-slug: changesmovieshistorywithentity-get
  description: Same as /Changes/Movies/History but with the specific entities that
    have changed inside the MovieResponse.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesmovieshistorywithentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesmovieshistorywithentity-get-openapi.md
- name: Entertainment Express - Returns list of unique PersonId changes greater than
    or equal to date (UTC).
  x-api-slug: changespeoplehistory-get
  description: Requires a valid Date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changespeoplehistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changespeoplehistory-get-openapi.md
- name: Entertainment Express - Returns list of unique PersonId and Entity changes
    greater than or equal to date (UTC).
  x-api-slug: changespeoplehistorywithentity-get
  description: Requires a valid Date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changespeoplehistorywithentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changespeoplehistorywithentity-get-openapi.md
- name: Entertainment Express - Returns list of unique SeasonId changes greater than
    or equal to date (UTC).
  x-api-slug: changesseasonshistory-get
  description: Use if you want to check for specific updates to season records.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesseasonshistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesseasonshistory-get-openapi.md
- name: Entertainment Express - Returns list of unique SeasonId and Entity changes
    greater than or equal to date (UTC).
  x-api-slug: changesseasonshistorywithentity-get
  description: Returns list of new or changed SeasonIds with the entity that has changed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesseasonshistorywithentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesseasonshistorywithentity-get-openapi.md
- name: Entertainment Express - Returns list of unique ShowId changes greater than
    or equal to date (UTC).
  x-api-slug: changesshowshistory-get
  description: All new and updated shows from requested date and time.  When a record
    gets updated, use the ID to get the full show object and replace the data in your
    cache.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesshowshistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesshowshistory-get-openapi.md
- name: Entertainment Express - Returns list of unique ShowId and Entity changes greater
    than or equal to date (UTC).
  x-api-slug: changesshowshistorywithentity-get
  description: Returns a list of ShowId and entity of any show that has been updated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesshowshistorywithentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/changes/master/_listings/entertainment-express/changesshowshistorywithentity-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://emuseum.api.docs.api.gallery.streamdata.io
- type: x-api-stack
  url: http://entertainment.express.stack.network
- type: x-blog
  url: https://www.internetvideoarchive.com/blog/
- type: x-developer
  url: https://developer.iva-api.com/
- type: x-pricing
  url: https://www.internetvideoarchive.com/pricing/
- type: x-website
  url: https://www.internetvideoarchive.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---