---
swagger: "2.0"
x-collection-name: Wordnik
x-complete: 1
info:
  title: Wordnik
  description: wordnik-is-the-worlds-biggest-online-english-dictionary-by-number-of-words
  version: "4.0"
host: api.wordnik.com
basePath: /v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account.json/wordLists:
    get:
      summary: Fetches WordList objects for the logged-in user.
      description: Fetches wordlist objects for the logged-in user..
      operationId: getWordListsForLoggedInUser
      x-api-path-slug: account-jsonwordlists-get
      parameters:
      - in: header
        name: auth_token
        description: auth_token of logged-in user
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: skip
        description: Results to skip
      responses:
        200:
          description: OK
      tags:
      - Account
      - Words
      - Lists
---