---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Fetch a fulfillment event.
  description: Fetch a fulfillment event..
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4528049998/fulfillments/3770145678/events/#{event_id}.json:
    get:
      summary: Fetch a fulfillment event.
      description: Fetch a fulfillment event..
      operationId: getAdminOrders4528049998Fulfillments3770145678Events#Event.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678eventsevent-id-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: event_id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Fetch
      - Fulfillment
      - Event
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