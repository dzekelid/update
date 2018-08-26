---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Update
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: The Confluence Cloud REST API - Create or update attachment
  x-api-slug: contentidchildattachment-put
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/contentidchildattachment-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/contentidchildattachment-put-openapi.md
- name: Jira Cloud REST API - Create or update remote issue link
  x-api-slug: api2issueissueidorkeyremotelink-post
  description: Creates or updates a remote issue link from a JSON representation.
    If a `globalId` is provided and a remote issue link exists with that globalId,
    the remote issue link is updated. Otherwise, the remote issue link is created.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2issueissueidorkeyremotelink-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2issueissueidorkeyremotelink-post-openapi.md
- name: Jira Cloud REST API - Partial update project role
  x-api-slug: api2roleid-post
  description: |-
    Update either the project role's name or its description.

    You cannot update both the name and description at the same time using this method. If you send a request with both a name and a description, then only the name will be updated, regardless of the order of appearance in the body of the request.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2roleid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2roleid-post-openapi.md
- name: Jira Cloud REST API - Fully update project role
  x-api-slug: api2roleid-put
  description: |-
    Update the project role's name and description. You must include both a name and a description in the request.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2roleid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2roleid-put-openapi.md
- name: Jira Cloud REST API - Create or update remote version link
  x-api-slug: api2versionversionidremotelink-post
  description: Create a remote version link via POST. The link's global ID will be
    taken from the JSON payload if provided; otherwise, it will be generated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2versionversionidremotelink-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2versionversionidremotelink-post-openapi.md
- name: Jira Cloud REST API - Create or update remote version link with global id
  x-api-slug: api2versionversionidremotelinkglobalid-post
  description: Create a remote version link via POST using the provided global ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2versionversionidremotelinkglobalid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/api2versionversionidremotelinkglobalid-post-openapi.md
- name: Stride API - Create or update a chat:actionTarget module
  x-api-slug: sitecloudidconversationconversationidappmodulechatactiontargetkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatactiontargetkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatactiontargetkey-put-openapi.md
- name: Stride API - Create or update a chat:bot module
  x-api-slug: sitecloudidconversationconversationidappmodulechatbotkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatbotkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatbotkey-put-openapi.md
- name: Stride API - Create or update a chat:bot:messages module
  x-api-slug: sitecloudidconversationconversationidappmodulechatbotmessageskey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatbotmessageskey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatbotmessageskey-put-openapi.md
- name: Stride API - Create or update a chat:dialog module
  x-api-slug: sitecloudidconversationconversationidappmodulechatdialogkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatdialogkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatdialogkey-put-openapi.md
- name: Stride API - Create or update a chat:externalPage module
  x-api-slug: sitecloudidconversationconversationidappmodulechatexternalpagekey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatexternalpagekey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatexternalpagekey-put-openapi.md
- name: Stride API - Create or update a chat:glance module
  x-api-slug: sitecloudidconversationconversationidappmodulechatglancekey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatglancekey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatglancekey-put-openapi.md
- name: Stride API - Create or update a chat:sidebar module
  x-api-slug: sitecloudidconversationconversationidappmodulechatsidebarkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatsidebarkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatsidebarkey-put-openapi.md
- name: Stride API - Create or update a chat:webhook module
  x-api-slug: sitecloudidconversationconversationidappmodulechatwebhookkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatwebhookkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatwebhookkey-put-openapi.md
- name: Stride API - Create or update a chat:actionTarget module
  x-api-slug: sitecloudidconversationconversationidappmodulechatactiontargetkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatactiontargetkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatactiontargetkey-put-openapi.md
- name: Stride API - Create or update a chat:bot module
  x-api-slug: sitecloudidconversationconversationidappmodulechatbotkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatbotkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatbotkey-put-openapi.md
- name: Stride API - Create or update a chat:bot:messages module
  x-api-slug: sitecloudidconversationconversationidappmodulechatbotmessageskey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatbotmessageskey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatbotmessageskey-put-openapi.md
- name: Stride API - Create or update a chat:dialog module
  x-api-slug: sitecloudidconversationconversationidappmodulechatdialogkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatdialogkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatdialogkey-put-openapi.md
- name: Stride API - Create or update a chat:externalPage module
  x-api-slug: sitecloudidconversationconversationidappmodulechatexternalpagekey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatexternalpagekey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatexternalpagekey-put-openapi.md
- name: Stride API - Create or update a chat:glance module
  x-api-slug: sitecloudidconversationconversationidappmodulechatglancekey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatglancekey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatglancekey-put-openapi.md
- name: Stride API - Create or update a chat:sidebar module
  x-api-slug: sitecloudidconversationconversationidappmodulechatsidebarkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatsidebarkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatsidebarkey-put-openapi.md
- name: Stride API - Create or update a chat:webhook module
  x-api-slug: sitecloudidconversationconversationidappmodulechatwebhookkey-put
  description: Authentication required, with scope participate:conversation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatwebhookkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/update/master/_listings/atlassian/sitecloudidconversationconversationidappmodulechatwebhookkey-put-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---