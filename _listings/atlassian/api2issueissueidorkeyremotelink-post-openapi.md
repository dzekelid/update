---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Create or update remote issue link
  description: Creates or updates a remote issue link from a JSON representation.
    If a `globalId` is provided and a remote issue link exists with that globalId,
    the remote issue link is updated. Otherwise, the remote issue link is created.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issue/{issueIdOrKey}/remotelink:
    post:
      summary: Create or update remote issue link
      description: Creates or updates a remote issue link from a JSON representation.
        If a `globalId` is provided and a remote issue link exists with that globalId,
        the remote issue link is updated. Otherwise, the remote issue link is created.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.createOrUpdateRemoteIssueLink_post
      x-api-path-slug: api2issueissueidorkeyremotelink-post
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to create/update the remote issue link
          for
      responses:
        200:
          description: OK
      tags:
      - Update
      - Remote
      - Issue
      - Link
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