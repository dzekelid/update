---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get_replies_by_last_update
  description: get_replies_by_last_update
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /witness_update:
    get:
      summary: witness_update
      description: witness_update
      operationId: witness-update
      x-api-path-slug: witness-update-get
      parameters:
      - in: query
        name: block_signing_key
        description: block_signing_key
      - in: query
        name: fee
        description: fee
      - in: query
        name: owner
        description: witness name
      - in: query
        name: props
        description: props
      - in: query
        name: url
        description: url
      responses:
        200:
          description: OK
      tags:
      - Witness
      - Update
  /get_replies_by_last_update:
    get:
      summary: get_replies_by_last_update
      description: get_replies_by_last_update
      operationId: get-replies-by-last-update
      x-api-path-slug: get-replies-by-last-update-get
      parameters:
      - in: query
        name: limit
        description: limit query
      - in: query
        name: startAuthor
        description: account name
      - in: query
        name: startPermlink
        description: permlink of post
      responses:
        200:
          description: OK
      tags:
      - Get
      - Replies
      - By
      - Last
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