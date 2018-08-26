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
  /admin/pages/216307854.json:
    put:
      summary: update a page
      description: Update a page.
      operationId: putAdminPages216307854.json
      x-api-path-slug: adminpages216307854-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Update
      - Page
  /admin/custom_collections/246409795.json:
    put:
      summary: update a custom collection
      description: Update a custom collection.
      operationId: putAdminCustomCollections246409795.json
      x-api-path-slug: admincustom-collections246409795-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Update
      - Custom
      - Collection
  /admin/countries/444574734.json:
    put:
      summary: update a country
      description: Update a country.
      operationId: putAdminCountries444574734.json
      x-api-path-slug: admincountries444574734-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Update
      - Country
  /admin/script_tags/108074126.json:
    put:
      summary: update a script tag
      description: Update a script tag.
      operationId: putAdminScriptTags108074126.json
      x-api-path-slug: adminscript-tags108074126-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Update
      - Script
      - Tag
---