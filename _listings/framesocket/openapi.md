---
swagger: "2.0"
x-collection-name: Framesocket
x-complete: 1
info:
  title: Framesocket
  description: framesocket-is-the-best-way-for-developers-and-content-owners-to-tackle-video-projects-of-any-size-
  version: 1.0.0
host: www.framesocket.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/update.php:
    get:
      summary: Update Media
      description: Update Media
      operationId: getMediaUpdate.php
      x-api-path-slug: mediaupdate-php-get
      parameters:
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: description
        description: Text String - Limit 1000 characters
      - in: query
        name: hash
        description: Video Hash
      - in: query
        name: imagehash
        description: This needs to refer to an image already assigned to this media
      - in: query
        name: key
        description: Your account username
      - in: query
        name: keywords
        description: Text String - Comma separated by keyword or phrase
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      - in: query
        name: title
        description: Text String - Limit 100 characters
      responses:
        200:
          description: OK
      tags:
      - Media
      - Update
---