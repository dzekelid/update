---
swagger: "2.0"
x-collection-name: SYNQ Video
x-complete: 1
info:
  title: SYNQ Video
  description: -sign-up-for-a-developer-api-keyhttpswww-synq-fmregister-synq-api-guide
  version: 1.9.1
host: api.synq.fm
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /video/update:
    post:
      summary: Update a video's metadata.
      description: Update a video's metadata through JavaScript code. Only fields
        inside the "userdata" object can be set.
      operationId: update
      x-api-path-slug: videoupdate-post
      parameters:
      - in: formData
        name: api_key
      - in: formData
        name: source
        description: JavaScript code to execute on the video object
      - in: formData
        name: video_id
        description: The ID of the video whose metadata will be updated
      responses:
        200:
          description: OK
      tags:
      - Video
      - Update
---