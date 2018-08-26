---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /scim/v2/Users/{id}:
    put:
      summary: fully update/replace a user
      description: ""
      operationId: replaceUser
      x-api-path-slug: scimv2usersid-put
      parameters:
      - in: body
        name: body
        description: an existing user
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: user id
      responses:
        200:
          description: OK
      tags:
      - Fully
      - Update
      - Replace
      - User
---