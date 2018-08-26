---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Fetch a team template
  description: Fetches a team template, by ID only.
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
  /v2/activities/emails/{id}.json:
    get:
      summary: Fetch an email
      description: Fetches an email, by ID only.
      operationId: v2.activities.emails.id.json.get
      x-api-path-slug: v2activitiesemailsid-json-get
      parameters:
      - in: path
        name: id
        description: Email ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Email
  /v2/cadence_memberships/{id}.json:
    get:
      summary: Fetch a cadence membership
      description: Fetches a cadence membership, by ID only.
      operationId: v2.cadence_memberships.id.json.get
      x-api-path-slug: v2cadence-membershipsid-json-get
      parameters:
      - in: path
        name: id
        description: CadenceMembership ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Cadence
      - Membership
  /v2/cadences/{id}.json:
    get:
      summary: Fetch a cadence
      description: Fetches a cadence, by ID only.
      operationId: v2.cadences.id.json.get
      x-api-path-slug: v2cadencesid-json-get
      parameters:
      - in: path
        name: id
        description: Cadence ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Cadence
  /v2/call_data_records/{id}.json:
    get:
      summary: Fetch a call data record
      description: Fetches a call data record, by ID only.
      operationId: v2.call_data_records.id.json.get
      x-api-path-slug: v2call-data-recordsid-json-get
      parameters:
      - in: path
        name: id
        description: CallDataRecord ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Call
      - Data
      - Record
  /v2/crm_activities/{id}.json:
    get:
      summary: Fetch a crm activity
      description: Fetches a crm activity, by ID only.
      operationId: v2.crm_activities.id.json.get
      x-api-path-slug: v2crm-activitiesid-json-get
      parameters:
      - in: path
        name: id
        description: Crm activity ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Crm
      - Activity
  /v2/custom_fields/{id}.json:
    get:
      summary: Fetch a custom field
      description: Fetches a custom field, by ID only.
      operationId: v2.custom_fields.id.json.get
      x-api-path-slug: v2custom-fieldsid-json-get
      parameters:
      - in: path
        name: id
        description: Custom Field ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Custom
      - Field
  /v2/email_templates/{id}.json:
    get:
      summary: Fetch an email template
      description: Fetches an email template, by ID only.
      operationId: v2.email_templates.id.json.get
      x-api-path-slug: v2email-templatesid-json-get
      parameters:
      - in: path
        name: id
        description: EmailTemplate ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Email
      - Template
  /v2/imports/{id}.json:
    get:
      summary: Fetch an import
      description: |-
        Fetches an import, by ID only.

        Admin users can access imports for the entire team, but non-admin users can only access their own imports.
      operationId: v2.imports.id.json.get
      x-api-path-slug: v2importsid-json-get
      parameters:
      - in: path
        name: id
        description: Import ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Import
  /v2/me.json:
    get:
      summary: Fetch current user
      description: |-
        Authenticated user information. This endpoint does not accept any parameters as it is
        represents your authenticated user. The "Users" resource provides user information
        for other users on the team.
      operationId: v2.me.json.get
      x-api-path-slug: v2me-json-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Current
      - User
  /v2/notes/{id}.json:
    get:
      summary: Fetch a note
      description: Fetches a note, by ID only.
      operationId: v2.notes.id.json.get
      x-api-path-slug: v2notesid-json-get
      parameters:
      - in: path
        name: id
        description: Note ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Note
  /v2/people/{id}.json:
    get:
      summary: Fetch a person
      description: Fetches a person, by ID only.
      operationId: v2.people.id.json.get
      x-api-path-slug: v2peopleid-json-get
      parameters:
      - in: path
        name: id
        description: Person ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Person
  /v2/person_stages/{id}.json:
    get:
      summary: Fetch a person stage
      description: Fetches a person stage, by ID only.
      operationId: v2.person_stages.id.json.get
      x-api-path-slug: v2person-stagesid-json-get
      parameters:
      - in: path
        name: id
        description: Stage ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Person
      - Stage
  /v2/phone_numbers/recording_settings/{id}.json:
    get:
      summary: Fetch recording setting
      description: |-
        Fetches the recording status for a given phone number, based on Do Not Record and Recording Governance for your team.
        Phone number should be in E.164 format.
      operationId: v2.phone_numbers.recording_settings.id.json.get
      x-api-path-slug: v2phone-numbersrecording-settingsid-json-get
      parameters:
      - in: path
        name: id
        description: E
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Recording
      - Setting
  /v2/steps/{id}.json:
    get:
      summary: Fetch a step
      description: Fetches a step, by ID only.
      operationId: v2.steps.id.json.get
      x-api-path-slug: v2stepsid-json-get
      parameters:
      - in: path
        name: id
        description: Step ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Step
  /v2/team.json:
    get:
      summary: Fetch current team
      description: Fetches the team of the authenticated user.
      operationId: v2.team.json.get
      x-api-path-slug: v2team-json-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Current
      - Team
  /v2/team_templates/{id}.json:
    get:
      summary: Fetch a team template
      description: Fetches a team template, by ID only.
      operationId: v2.team_templates.id.json.get
      x-api-path-slug: v2team-templatesid-json-get
      parameters:
      - in: path
        name: id
        description: Team Template ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Team
      - Template
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