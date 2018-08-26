---
swagger: "2.0"
x-collection-name: OpenCorporates
x-complete: 1
info:
  title: OpenCorporates
  description: the-api-for-managing-opencorporates-data-
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
---