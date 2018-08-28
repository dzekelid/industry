---
swagger: "2.0"
x-collection-name: OpenCorporates
x-complete: 0
info:
  title: OpenCorporates Industry Codes  Code Scheme ID
  description: nThis call returns further details about the code_scheme, together
    with the list of industry codes associated with it
  termsOfService: https://opencorporates.com/info/licence
  version: v.04
host: api.opencorporates.com
basePath: v0.4/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /industry_codes/:code_scheme_id:
    get:
      summary: Industry Codes  Code Scheme ID
      description: nThis call returns further details about the code_scheme, together
        with the list of industry codes associated with it
      operationId: get-industry-codes--code-scheme-id
      x-api-path-slug: industry-codescode-scheme-id-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Industry
      - Codes
      - :code
      - Scheme
      - Id
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