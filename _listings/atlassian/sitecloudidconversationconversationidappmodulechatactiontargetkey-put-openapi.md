---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Software Cloud API Create or update a chat:actionTarget module
  description: Authentication required, with scope participate:conversation
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:actionTarget/{key}:
    put:
      summary: Create or update a chat:actionTarget module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatActionTargetPutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatactiontargetkey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:actionTarget
      - Module
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