---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Partial update project role
  description: |-
    Update either the project role's name or its description.

    You cannot update both the name and description at the same time using this method. If you send a request with both a name and a description, then only the name will be updated, regardless of the order of appearance in the body of the request.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
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
  /api/2/role/{id}:
    post:
      summary: Partial update project role
      description: |-
        Update either the project role's name or its description.

        You cannot update both the name and description at the same time using this method. If you send a request with both a name and a description, then only the name will be updated, regardless of the order of appearance in the body of the request.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.RoleResource.partialUpdateProjectRole_post
      x-api-path-slug: api2roleid-post
      parameters:
      - in: path
        name: id
        description: The ID of the project role
      responses:
        200:
          description: OK
      tags:
      - Partial
      - Update
      - Project
      - Role
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