---
name: Public Transport Victoria Timetable
x-slug: public-transport-victoria-timetable
description: The PTV Timetable API provides direct access to Public Transport Victoria&rsquo;s
  public transport timetable data. The API returns scheduled timetable, route and
  stop data for all metropolitan and regional train, tram and bus services in Victoria,
  including Night Network(Night Train and Night Tram data are included in metropolitan
  train and tram services data, respectively, whereas Night Bus is a separate route
  type). The API also returns real-time data for metropolitan train, tram and bus
  services (where this data is made available to PTV), as well as disruption information,
  stop facility information, and access to myki ticket outlet data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/public-transport-victoria.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Run
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/run/master/_listings/public-transport-victoria-timetable/apis.md
specificationVersion: "0.14"
apis:
- name: Public Transport Victoria Timetable - Get V3 Pattern Run Run Route Type Route
    Type
  x-api-slug: v3patternrunrun-idroute-typeroute-type-get
  description: View the stopping pattern for a specific trip/service run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/public-transport-victoria.png
  humanURL: https://www.ptv.vic.gov.au/about-ptv/data-and-reports/datasets/ptv-timetable-api/
  baseURL: https://timetableapi.ptv.vic.gov.au//
  tags: Transit, API Provider, Transportation, Profiles, General Data, Cities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/run/master/_listings/public-transport-victoria-timetable/v3patternrunrun-idroute-typeroute-type-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/run/master/_listings/public-transport-victoria-timetable/v3patternrunrun-idroute-typeroute-type-get-openapi.md
- name: Public Transport Victoria Timetable - Get V3 Runs Run
  x-api-slug: v3runsrun-id-get
  description: View all trip/service runs for a specific run id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/public-transport-victoria.png
  humanURL: https://www.ptv.vic.gov.au/about-ptv/data-and-reports/datasets/ptv-timetable-api/
  baseURL: https://timetableapi.ptv.vic.gov.au//
  tags: Transit, API Provider, Transportation, Profiles, General Data, Cities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/run/master/_listings/public-transport-victoria-timetable/v3runsrun-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/run/master/_listings/public-transport-victoria-timetable/v3runsrun-id-get-openapi.md
- name: Public Transport Victoria Timetable - Get V3 Runs Run Route Type Route Type
  x-api-slug: v3runsrun-idroute-typeroute-type-get
  description: View the trip/service run for a specific run id and route type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/public-transport-victoria.png
  humanURL: https://www.ptv.vic.gov.au/about-ptv/data-and-reports/datasets/ptv-timetable-api/
  baseURL: https://timetableapi.ptv.vic.gov.au//
  tags: Transit, API Provider, Transportation, Profiles, General Data, Cities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/run/master/_listings/public-transport-victoria-timetable/v3runsrun-idroute-typeroute-type-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/run/master/_listings/public-transport-victoria-timetable/v3runsrun-idroute-typeroute-type-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://product.hunt.api.gallery.streamdata.io
- type: x-api-stack
  url: http://public.transport.victoria.timetable.stack.network
- type: x-website
  url: https://www.ptv.vic.gov.au/about-ptv/data-and-reports/datasets/ptv-timetable-api/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---