---
swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 0
info:
  title: Ge.tt  REST API Shares Update
  description: Updates a share. Currently you can only update the title
  termsOfService: http://ge.tt/terms
  version: "1"
host: open.ge.tt
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1/shares/{sharename}/update:
    post:
      summary: Shares Update
      description: Updates a share. Currently you can only update the title
      operationId: post1SharesSharenameUpdate
      x-api-path-slug: 1sharessharenameupdate-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Sharename
      - Update
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