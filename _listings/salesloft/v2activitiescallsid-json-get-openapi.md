---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Fetch a call
  description: Fetches a call, by ID only.
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/accounts/{id}.json:
    get:
      summary: Fetch an account
      description: Fetches an account, by ID only.
      operationId: v2.accounts.id.json.get
      x-api-path-slug: v2accountsid-json-get
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Account
  /v2/action_details/call_instructions/{id}.json:
    get:
      summary: Fetch a call instructions
      description: Fetches a call instruction, by ID only.
      operationId: v2.action_details.call_instructions.id.json.get
      x-api-path-slug: v2action-detailscall-instructionsid-json-get
      parameters:
      - in: path
        name: id
        description: Call instructions ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Call
      - Instructions
  /v2/actions/{id}.json:
    get:
      summary: Fetch an action
      description: |-
        Fetches an action, by ID only.
        This endpoint will only return actions that are in_progress or pending_activity.
        Once an action is complete, the request for that action will return a 404 status code.
      operationId: v2.actions.id.json.get
      x-api-path-slug: v2actionsid-json-get
      parameters:
      - in: path
        name: id
        description: Action ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Action
  /v2/activities/calls/{id}.json:
    get:
      summary: Fetch a call
      description: Fetches a call, by ID only.
      operationId: v2.activities.calls.id.json.get
      x-api-path-slug: v2activitiescallsid-json-get
      parameters:
      - in: path
        name: id
        description: Call ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Call
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