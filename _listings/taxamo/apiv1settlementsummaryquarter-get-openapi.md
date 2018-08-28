---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 0
info:
  title: Taxamo Fetch Summary
  description: Fetch summary.
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/settlement/refunds:
    get:
      summary: Fetch Refunds
      description: Fetch refunds.
      operationId: getRefunds
      x-api-path-slug: apiv1settlementrefunds-get
      parameters:
      - in: query
        name: date_from
        description: Take only refunds issued at or after the date
      - in: query
        name: format
        description: Output format
      - in: query
        name: moss_country_code
        description: MOSS country code, used to determine currency
      - in: query
        name: tax_region
        description: Tax region key, defaults to EU for backwards compatibility
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Refunds
  /api/v1/settlement/summary/{quarter}:
    get:
      summary: Fetch Summary
      description: Fetch summary.
      operationId: getSettlementSummary
      x-api-path-slug: apiv1settlementsummaryquarter-get
      parameters:
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: moss_country_code
        description: MOSS country code, used to determine currency
      - in: path
        name: quarter
        description: Quarter in yyyy-MM format
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      - in: query
        name: tax_region
        description: Tax region key
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Summary
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