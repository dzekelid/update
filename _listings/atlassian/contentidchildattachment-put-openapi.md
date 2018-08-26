---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Create or update attachment
  description: "Adds an attachment to a piece of content. If the attachment already
    exists \nfor the content, then the attachment is updated (i.e. a new version of
    the \nattachment is created).\n\nNote, you must set a `X-Atlassian-Token: nocheck`
    header on the request \nfor this method, otherwise it will be blocked. This protects
    against XSRF \nattacks, which is necessary as this method accepts multipart/form-data.\n\nThe
    media type 'multipart/form-data' is defined in [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt).
    \nMost client libraries have classes that make it easier to implement \nmultipart
    posts, like the [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
    \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
    attaches a file ('example.txt') to a piece of \ncontent (id='123') with a comment
    and `minorEdits`=true. If the 'example.txt' \nfile already exists, it will update
    it with a new version of the attachment.\n\n``` bash\ncurl -D- \\\n  -u admin:admin
    \\\n  -X PUT \\\n  -H \"X-Atlassian-Token: nocheck\" \\\n  -F \"file=@example.txt\"
    \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example attachment comment\" \\\n
    \ http://myhost/rest/api/content/123/child/attachment\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
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
  /content/{id}/child/attachment:
    put:
      summary: Create or update attachment
      description: "Adds an attachment to a piece of content. If the attachment already
        exists \nfor the content, then the attachment is updated (i.e. a new version
        of the \nattachment is created).\n\nNote, you must set a `X-Atlassian-Token:
        nocheck` header on the request \nfor this method, otherwise it will be blocked.
        This protects against XSRF \nattacks, which is necessary as this method accepts
        multipart/form-data.\n\nThe media type 'multipart/form-data' is defined in
        [RFC 1867](https://www.ietf.org/rfc/rfc1867.txt). \nMost client libraries
        have classes that make it easier to implement \nmultipart posts, like the
        [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html)
        \nJava class provided by Apache HTTP Components.\n\nExample: This curl command
        attaches a file ('example.txt') to a piece of \ncontent (id='123') with a
        comment and `minorEdits`=true. If the 'example.txt' \nfile already exists,
        it will update it with a new version of the attachment.\n\n``` bash\ncurl
        -D- \\\n  -u admin:admin \\\n  -X PUT \\\n  -H \"X-Atlassian-Token: nocheck\"
        \\\n  -F \"file=@example.txt\" \\\n  -F \"minorEdit=true\" \\\n  -F \"comment=Example
        attachment comment\" \\\n  http://myhost/rest/api/content/123/child/attachment\n```\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.AttachmentResource.createOrUpdateAttachments_put
      x-api-path-slug: contentidchildattachment-put
      parameters:
      - in: path
        name: id
        description: The ID of the content to add the attachment to
      - in: query
        name: status
        description: The status of the content that the attachment is being added
          to
      responses:
        200:
          description: OK
      tags:
      - Update
      - Attachment
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