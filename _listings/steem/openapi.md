---
swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
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
---