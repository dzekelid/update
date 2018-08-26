---
swagger: "2.0"
x-collection-name: Viddler
x-complete: 0
info:
  title: Viddler  API Logins Update
  description: Updates a current login.
  termsOfService: http://www.viddler.com/terms-of-use/
  version: v2
host: api.viddler.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  viddler.logins.update:
    post:
      summary: Logins Update
      description: Updates a current login.
      operationId: logins-update
      x-api-path-slug: viddler-logins-update-post
      parameters:
      - in: query
        name: analytics_permissions
        description: 'options: manage'
      - in: query
        name: api_access_permissions
        description: 'options: manage'
      - in: query
        name: api_settings_permissions
        description: 'options: manage'
      - in: query
        name: billing_settings_permissions
        description: 'options: manage'
      - in: query
        name: branding_settings_permissions
        description: 'options: manage'
      - in: query
        name: email
        description: The email of the user
      - in: query
        name: encoding_settings_permissions
        description: 'options: manage'
      - in: query
        name: interaction_settings_permissions
        description: 'options: manage'
      - in: query
        name: invoices_permissions
        description: 'options: manage'
      - in: query
        name: itunes_settings_permissions
        description: 'options: manage'
      - in: query
        name: login
        description: The login username you would like to create
      - in: query
        name: logins_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: name
        description: The name of the user
      - in: query
        name: password
        description: The password of the user
      - in: query
        name: player_settings_permissions
        description: 'options: manage'
      - in: query
        name: playlists_permissions
        description: 'options: manage'
      - in: query
        name: playlist_ids
        description: A comma delimited list of playlist IDs this user can view
      - in: query
        name: privacy_settings_permissions
        description: 'options: manage'
      - in: query
        name: profile_permissions
        description: 'options: manage'
      - in: query
        name: recorder_permissions
        description: 'options: manage'
      - in: query
        name: sessionid
      - in: query
        name: subaccounts_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: support_permissions
        description: 'options: manage'
      - in: query
        name: videos_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: vidgets_permissions
        description: 'options: manage'
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Logins
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