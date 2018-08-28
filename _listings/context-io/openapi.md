swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/messages/{message_id}/body:
    get:
      summary: Get Accounts Messages Message Body
      description: 'Fetches the message body of a given email. On-demand data retrieval:
        since we do not keep full copies of emails on our servers, this call triggers
        a connection to the IMAP server to fetch the message. One thing to point out
        is we do fetch messages in such a way that large files attached to a message
        won''t make any difference in the response time. This call only returns text
        portions of messages, attachments aren''t included. To get a list of attachments
        on the message, look for the files property in the response of a message instance.
        To download the content of these attachments, use the files/content call.'
      operationId: getAccountMessageBody_
      x-api-path-slug: accountsidmessagesmessage-idbody-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      - in: query
        name: type
        description: Many emails are sent with both rich text and plain text versions
          in the message body and by default, the response of this call will include
          both
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Body
  /accounts/{id}/messages/{message_id}/source:
    get:
      summary: Get Accounts Messages Message Source
      description: 'Fetches the message source. Returns the raw RFC-822 message source
        for the message (including attachments) with no parsing or decoding to any
        portions of the message. On-demand data retrieval: since we do not keep full
        copies of emails on our servers, this call triggers a connection to the IMAP
        server to fetch the message. Attachments are part of the message source so
        they will impact how fast this call responds.'
      operationId: getAccountMessageSource_
      x-api-path-slug: accountsidmessagesmessage-idsource-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Source