swagger: "2.0"
x-collection-name: Quovo
x-complete: 1
info:
  title: Quovo API v3
  description: todo-add-description
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
  /accounts:
    get:
      summary: Get all accounts
      description: Fetches all Accounts accross all Users.
      operationId: AccountsGet
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{account_id}/holdings:
    get:
      summary: Get an account's holdings
      description: Fetches all holdings for a specific account.
      operationId: AccountsHoldingsByAccountIdGet
      x-api-path-slug: accountsaccount-idholdings-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Holdings