---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 1
info:
  title: Watchful
  description: watchful-resulted-from-the-need-for-a-single-unified-dashboard-to-easily-monitor-all-of-the-web-sites-in-our-portfolios--after-years-of-evolution-our-solution-has-matured-into-a-simple-complete-and-professional-service--
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /extensions/{id}/update:
    post:
      summary: Update The Extension On The Remote Site
      description: Update the extension on the remote site
      operationId: updateExtension
      x-api-path-slug: extensionsidupdate-post
      parameters:
      - in: path
        name: id
        description: ID of the extension
      responses:
        200:
          description: OK
      tags:
      - Extensions
      - Id
      - Update
---