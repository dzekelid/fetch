---
swagger: "2.0"
x-collection-name: National Renewable Energy Laboratory
x-complete: 0
info:
  title: Transportation Laws and Incentives Fetch the details of a specific law given
    the law's ID.
  description: Fetch the details of a specific law given the law's id..
  version: 0.1.0
host: developer.nrel.gov
basePath: /api/transportation-incentives-laws
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{id}.{output_format}:
    get:
      summary: Fetch the details of a specific law given the law's ID.
      description: Fetch the details of a specific law given the law's id..
      operationId: v1.id.output_format.get
      x-api-path-slug: v1id-output-format-get
      parameters:
      - in: path
        name: id
        description: The id of the law that you are searching
      - in: path
        name: output_format
        description: Response format
      - in: query
        name: poc
        description: Include points of contacts in the return value
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Details
      - Of
      - Specific
      - Law
      - Given
      - Laws
      - ID
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