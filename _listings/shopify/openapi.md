---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
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
---