swagger: "2.0"
x-collection-name: National Renewable Energy Laboratory
x-complete: 1
info:
  title: Transportation Laws and Incentives
  description: query-our-database-of-state-and-federal-laws-and-incentives-for-alternative-fuels
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