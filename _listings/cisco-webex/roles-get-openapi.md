---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: Webex Teams Admin API Get roles (to fetch a role id)
  description: |-
    List all roles.

    https://developer.webex.com/endpoint-roles-get.html

    Example Response:
    ``` json
    {
      'items' : [ {
        'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
        'displayName' : 'Full Administrator'
      } ]
    }
    ```
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /roles:
    get:
      summary: Get roles (to fetch a role id)
      description: |-
        List all roles.

        https://developer.webex.com/endpoint-roles-get.html

        Example Response:
        ``` json
        {
          'items' : [ {
            'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
            'displayName' : 'Full Administrator'
          } ]
        }
        ```
      operationId: RolesGet2
      x-api-path-slug: roles-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Roles
      - (to
      - Fetch
      - Role
      - Id)
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