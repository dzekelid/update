---
swagger: "2.0"
x-collection-name: SYNQ Video
x-complete: 0
info:
  title: SYNQ Video Update a video's metadata.
  description: Update a video's metadata through JavaScript code. Only fields inside
    the "userdata" object can be set.
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