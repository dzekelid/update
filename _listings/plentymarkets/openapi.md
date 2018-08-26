---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /rest/items/variations/variation_categories:
    put:
      summary: Bulk update category links
      description: Updates up to 50 links between variations and categories. The ID
        of the variations and the ID of the categories must be specified.
      operationId: putRestItemsVariationsVariationCategories
      x-api-path-slug: restitemsvariationsvariation-categories-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Category
      - Links
  /rest/items/variations/variation_properties:
    post:
      summary: Bulk update properties
      description: Creates up to 50 properties of variations.
      operationId: postRestItemsVariationsVariationProperties
      x-api-path-slug: restitemsvariationsvariation-properties-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Properties
    put:
      summary: Bulk update properties
      description: Updates up to 50 properties of variations.
      operationId: putRestItemsVariationsVariationProperties
      x-api-path-slug: restitemsvariationsvariation-properties-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Properties
  /rest/items/variations/variation_sales_prices:
    put:
      summary: Bulk update prices
      description: Updates up to 50 prices of variations. The ID of the variation,
        the ID of the sales price and a price must be specified.
      operationId: putRestItemsVariationsVariationSalesPrices
      x-api-path-slug: restitemsvariationsvariation-sales-prices-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_sales_prices
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Prices
---