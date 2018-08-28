---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Master Get Master By Global Industry
  description: Get master records by industry.
  version: 1.0.0
host: globalmaster.xignite.com
basePath: xglobalmaster.json/XigniteGlobalMaster
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetTopIndustryHeadlines:
    get:
      summary: Get Top Industry Headlines
      description: Return the top press releases for an industry.
      operationId: postGettopindustryheadlines
      x-api-path-slug: gettopindustryheadlines-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Industry
      - Headlines
  /GetTodaysIndustryHeadlines:
    get:
      summary: Get Todays Industry Headlines
      description: Return press releases for today for an industry.
      operationId: postGettodaysindustryheadlines
      x-api-path-slug: gettodaysindustryheadlines-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Todays
      - Industry
      - Headlines
  /GetLastIndustryHeadlines:
    get:
      summary: Get Last Industry Headlines
      description: Return the last press releases since a certain time for an industry.
      operationId: postGetlastindustryheadlines
      x-api-path-slug: getlastindustryheadlines-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Industry
      - Headlines
  /GetMasterByIndustry:
    get:
      summary: Get Master By Industry
      description: Old version of the service. Customers should use GetMasterByGlobalIndustry
      operationId: GetMasterByIndustry
      x-api-path-slug: getmasterbyindustry-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Industry
  /GetMasterByGlobalIndustry:
    get:
      summary: Get Master By Global Industry
      description: Get master records by industry.
      operationId: GetMasterByGlobalIndustry
      x-api-path-slug: getmasterbyglobalindustry-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Global
      - Industry
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