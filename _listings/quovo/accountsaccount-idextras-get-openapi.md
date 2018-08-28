---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 0
info:
  title: Quovo Fetch an Account's Extras Information
  description: Retrieves an Account's Extras Information.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /connections/{connection_id}/accounts:
    get:
      summary: Fetch the Connection's Accounts
      description: |-
        Fetches all of the accounts belonging to the connection. These are automatically created by Quovo after an initial sync.

        If you have a Postman Environment set up, this request will automatically set the variable `account_id` to the id of the first account returned.
      operationId: ConnectionsAccountsByConnectionIdGet4
      x-api-path-slug: connectionsconnection-idaccounts-get
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Connections
      - Accounts
  /accounts/{account_id}/extras:
    get:
      summary: Fetch an Account's Extras Information
      description: Retrieves an Account's Extras Information.
      operationId: AccountsExtrasByAccountIdGet
      x-api-path-slug: accountsaccount-idextras-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Accounts
      - Extras
      - Information
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