---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Caption Captionasset Action Update
  description: Update caption asset
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/accesscontrol/action/update:
    get:
      summary: Get Service Access Control Action Update
      description: Update Access Control Profile by id
      operationId: accessControl.update
      x-api-path-slug: serviceaccesscontrolactionupdate-get
      parameters:
      - in: query
        name: accessControl[description]
        description: The description of the Access Control Profile
      - in: query
        name: accessControl[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`True if this Conversion Profile
          is the default'
      - in: query
        name: accessControl[name]
        description: The name of the Access Control Profile
      - in: query
        name: accessControl[restrictions]
      - in: query
        name: accessControl[systemName]
        description: System name of the Access Control Profile
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrol
      - Action
      - Update
  /service/accesscontrolprofile/action/update:
    get:
      summary: Get Service Access Controlprofile Action Update
      description: Update access control profile by id
      operationId: accessControlProfile.update
      x-api-path-slug: serviceaccesscontrolprofileactionupdate-get
      parameters:
      - in: query
        name: accessControlProfile[description]
        description: The description of the Access Control Profile
      - in: query
        name: accessControlProfile[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`True if this access control
          profile is the partner default'
      - in: query
        name: accessControlProfile[name]
        description: The name of the Access Control Profile
      - in: query
        name: accessControlProfile[rules]
      - in: query
        name: accessControlProfile[systemName]
        description: System name of the Access Control Profile
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrolprofile
      - Action
      - Update
  /service/annotation_annotation/action/update:
    get:
      summary: Get Service Annotation Annotation Action Update
      description: Update annotation by id
      operationId: annotation.update
      x-api-path-slug: serviceannotation-annotationactionupdate-get
      parameters:
      - in: query
        name: annotation[adType]
        description: 'Enum Type: `KalturaAdType`'
      - in: query
        name: annotation[answerKey]
      - in: query
        name: annotation[assetId]
      - in: query
        name: annotation[code]
      - in: query
        name: annotation[correctAnswerKeys]
      - in: query
        name: annotation[description]
      - in: query
        name: annotation[duration]
        description: Duration in milliseconds
      - in: query
        name: annotation[endTime]
        description: End time in milliseconds
      - in: query
        name: annotation[entryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[eventType]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: annotation[explanation]
      - in: query
        name: annotation[forceStop]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: annotation[hint]
      - in: query
        name: annotation[isPublic]
        description: 'Enum Type: `KalturaNullableBoolean`Is the annotation public'
      - in: query
        name: annotation[objectType]
      - in: query
        name: annotation[optionalAnswers]
      - in: query
        name: annotation[parentId]
        description: '`insertOnly`'
      - in: query
        name: annotation[partnerData]
      - in: query
        name: annotation[partnerSortValue]
      - in: query
        name: annotation[protocolType]
        description: '`insertOnly`Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: annotation[question]
      - in: query
        name: annotation[quizUserEntryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[searchableOnEntry]
        description: 'Enum Type: `KalturaNullableBoolean`Should the cue point get
          indexed on the entry'
      - in: query
        name: annotation[sourceUrl]
      - in: query
        name: annotation[startTime]
        description: Start time in milliseconds
      - in: query
        name: annotation[subType]
        description: 'Enum Type: `KalturaThumbCuePointSubType`The sub type of the
          ThumbCuePoint'
      - in: query
        name: annotation[systemName]
      - in: query
        name: annotation[tags]
      - in: query
        name: annotation[text]
      - in: query
        name: annotation[thumbOffset]
      - in: query
        name: annotation[title]
      - in: query
        name: annotation[triggeredAt]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Update
  /service/apptoken/action/update:
    get:
      summary: Get Service Apptoken Action Update
      description: Update application authentication token by id
      operationId: appToken.update
      x-api-path-slug: serviceapptokenactionupdate-get
      parameters:
      - in: query
        name: appToken[expiry]
        description: Expiry time of current token (unix timestamp in seconds)
      - in: query
        name: appToken[hashType]
        description: 'Enum Type: `KalturaAppTokenHashType`'
      - in: query
        name: appToken[sessionDuration]
        description: Expiry duration of KS (Kaltura Session) that created using the
          current token (in seconds)
      - in: query
        name: appToken[sessionPrivileges]
        description: Comma separated privileges to be applied on KS (Kaltura Session)
          that created using the current token
      - in: query
        name: appToken[sessionType]
        description: 'Enum Type: `KalturaSessionType`Type of KS (Kaltura Session)
          that created using the current token'
      - in: query
        name: appToken[sessionUserId]
        description: User id of KS (Kaltura Session) that created using the current
          token
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Apptoken
      - Action
      - Update
  /service/attachment_attachmentasset/action/update:
    get:
      summary: Get Service Attachment Attachmentasset Action Update
      description: Update attachment asset
      operationId: attachmentAsset.update
      x-api-path-slug: serviceattachment-attachmentassetactionupdate-get
      parameters:
      - in: query
        name: attachmentAsset[accuracy]
        description: The accuracy of the transcript - values between 0 and 1
      - in: query
        name: attachmentAsset[actualSourceAssetParamsIds]
        description: Comma separated list of source flavor params ids
      - in: query
        name: attachmentAsset[fileExt]
        description: '`insertOnly`The file extension'
      - in: query
        name: attachmentAsset[filename]
        description: The filename of the attachment asset content
      - in: query
        name: attachmentAsset[format]
        description: 'Enum Type: `KalturaAttachmentType`The attachment format'
      - in: query
        name: attachmentAsset[humanVerified]
        description: 'Enum Type: `KalturaNullableBoolean`Was verified by human or
          machine'
      - in: query
        name: attachmentAsset[language]
        description: 'Enum Type: `KalturaLanguage`The language of the transcript'
      - in: query
        name: attachmentAsset[objectType]
      - in: query
        name: attachmentAsset[partnerData]
        description: Partner private data
      - in: query
        name: attachmentAsset[partnerDescription]
        description: Partner friendly description
      - in: query
        name: attachmentAsset[providerType]
        description: 'Enum Type: `KalturaTranscriptProviderType`The provider of the
          transcript'
      - in: query
        name: attachmentAsset[tags]
        description: Tags used to identify the Flavor Asset in various scenarios
      - in: query
        name: attachmentAsset[title]
        description: Attachment asset title
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Update
  /service/baseentry/action/update:
    get:
      summary: Get Service Baseentry Action Update
      description: Update base entry. Only the properties that were set will be updated.
      operationId: baseEntry.update
      x-api-path-slug: servicebaseentryactionupdate-get
      parameters:
      - in: query
        name: baseEntry[accessControlId]
        description: The Access Control ID assigned to this entry (null when not set,
          send -1 to remove)
      - in: query
        name: baseEntry[adminTags]
        description: Entry admin tags can be updated only by administrators
      - in: query
        name: baseEntry[bitrates]
      - in: query
        name: baseEntry[categoriesIds]
        description: Comma separated list of ids of categories to which this entry
          belongs
      - in: query
        name: baseEntry[categories]
        description: Comma separated list of full names of categories to which this
          entry belongs
      - in: query
        name: baseEntry[conversionProfileId]
        description: Override the default ingestion profile
      - in: query
        name: baseEntry[conversionQuality]
        description: '`insertOnly`Override the default conversion quality'
      - in: query
        name: baseEntry[creatorId]
        description: '`insertOnly`The ID of the user who created this entry'
      - in: query
        name: baseEntry[creditUrl]
        description: The URL for credits
      - in: query
        name: baseEntry[creditUserName]
        description: The user name used for credits
      - in: query
        name: baseEntry[currentBroadcastStartTime]
        description: The time (unix timestamp in milliseconds) in which the entry
          broadcast started or 0 when the entry is off the air
      - in: query
        name: baseEntry[dataContent]
        description: The data of the entry
      - in: query
        name: baseEntry[description]
        description: Entry description
      - in: query
        name: baseEntry[displayInSearch]
        description: 'Enum Type: `KalturaEntryDisplayInSearchType`should we display
          this entry in search'
      - in: query
        name: baseEntry[documentType]
        description: '`insertOnly`Enum Type: `KalturaDocumentType`The type of the
          document'
      - in: query
        name: baseEntry[dvrStatus]
        description: 'Enum Type: `KalturaDVRStatus`DVR Status Enabled/Disabled'
      - in: query
        name: baseEntry[dvrWindow]
        description: Window of time which the DVR allows for backwards scrubbing (in
          minutes)
      - in: query
        name: baseEntry[editorType]
        description: 'Enum Type: `KalturaEditorType`The editor type used to edit the
          metadata'
      - in: query
        name: baseEntry[encodingIP1]
        description: The broadcast primary ip
      - in: query
        name: baseEntry[encodingIP2]
        description: The broadcast secondary ip
      - in: query
        name: baseEntry[endDate]
        description: Entry scheduling end date (null when not set, send -1 to remove)
      - in: query
        name: baseEntry[entitledUsersEdit]
        description: list of user ids that are entitled to edit the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: baseEntry[entitledUsersPublish]
        description: list of user ids that are entitled to publish the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: baseEntry[externalSourceType]
        description: '`insertOnly`Enum Type: `KalturaExternalMediaSourceType`The source
          type of the external media'
      - in: query
        name: baseEntry[filters]
      - in: query
        name: baseEntry[groupId]
      - in: query
        name: baseEntry[hlsStreamUrl]
        description: HLS URL - URL for live stream playback on mobile device
      - in: query
        name: baseEntry[lastElapsedRecordingTime]
        description: Elapsed recording time (in msec) up to the point where the live
          stream was last stopped (unpublished)
      - in: query
        name: baseEntry[licenseType]
        description: 'Enum Type: `KalturaLicenseType`License type used for this entry'
      - in: query
        name: baseEntry[liveStreamConfigurations]
      - in: query
        name: baseEntry[mediaType]
        description: '`insertOnly`Enum Type: `KalturaMediaType`The media type of the
          entry'
      - in: query
        name: baseEntry[msDuration]
        description: The duration in miliseconds
      - in: query
        name: baseEntry[name]
        description: Entry name (Min 1 chars)
      - in: query
        name: baseEntry[objectType]
      - in: query
        name: baseEntry[offlineMessage]
        description: The message to be presented when the stream is offline
      - in: query
        name: baseEntry[operationAttributes]
      - in: query
        name: baseEntry[parentEntryId]
        description: ID of source root entry, used for defining entires association
      - in: query
        name: baseEntry[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: baseEntry[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: baseEntry[playlistContent]
        description: Content of the playlist - XML if the playlistType is dynamic
          text if the playlistType is static url if the playlistType is mRss
      - in: query
        name: baseEntry[playlistId]
        description: Playlist id to be played
      - in: query
        name: baseEntry[playlistType]
        description: 'Enum Type: `KalturaPlaylistType`Type of playlist'
      - in: query
        name: baseEntry[primaryBroadcastingUrl]
      - in: query
        name: baseEntry[primaryRtspBroadcastingUrl]
      - in: query
        name: baseEntry[publishConfigurations]
      - in: query
        name: baseEntry[pushPublishEnabled]
        description: 'Enum Type: `KalturaLivePublishStatus`Flag denoting whether entry
          should be published by the media server'
      - in: query
        name: baseEntry[recordedEntryId]
        description: Recorded entry id
      - in: query
        name: baseEntry[recordingOptions][shouldCopyEntitlement]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: baseEntry[recordingOptions][shouldCopyScheduling]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: baseEntry[recordingOptions][shouldCopyThumbnail]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: baseEntry[recordingOptions][shouldMakeHidden]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: baseEntry[recordStatus]
        description: 'Enum Type: `KalturaRecordStatus`Recording Status Enabled/Disabled'
      - in: query
        name: baseEntry[redirectEntryId]
        description: IF not empty, points to an entry ID the should replace this current
          entrys id
      - in: query
        name: baseEntry[referenceId]
        description: Entry external reference id
      - in: query
        name: baseEntry[repeat]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that the segments
          should be repeated for ever'
      - in: query
        name: baseEntry[retrieveDataContentByGet]
        description: '`insertOnly`indicator whether to return the object for get action
          with the dataContent field'
      - in: query
        name: baseEntry[searchProviderId]
        description: '`insertOnly`The ID of the media in the importing site'
      - in: query
        name: baseEntry[searchProviderType]
        description: '`insertOnly`Enum Type: `KalturaSearchProviderType`The search
          provider type used to import this entry'
      - in: query
        name: baseEntry[secondaryBroadcastingUrl]
      - in: query
        name: baseEntry[secondaryRtspBroadcastingUrl]
      - in: query
        name: baseEntry[sourceType]
        description: '`insertOnly`Enum Type: `KalturaSourceType`The source type of
          the entry'
      - in: query
        name: baseEntry[startDate]
        description: Entry scheduling start date (null when not set, send -1 to remove)
      - in: query
        name: baseEntry[streamName]
      - in: query
        name: baseEntry[streamPassword]
        description: The broadcast password
      - in: query
        name: baseEntry[streams]
      - in: query
        name: baseEntry[streamUrl]
        description: The stream url
      - in: query
        name: baseEntry[tags]
        description: Entry tags
      - in: query
        name: baseEntry[templateEntryId]
        description: '`insertOnly`Template entry id'
      - in: query
        name: baseEntry[totalResults]
        description: Maximum count of results to be returned in playlist execution
      - in: query
        name: baseEntry[type]
        description: 'Enum Type: `KalturaEntryType`The type of the entry, this is
          auto filled by the derived entry object'
      - in: query
        name: baseEntry[urlManager]
        description: URL Manager to handle the live stream URL (for instance, add
          token)
      - in: query
        name: baseEntry[userId]
        description: The ID of the user who is the owner of this entry
      - in: query
        name: entryId
        description: Entry id to update
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Update
  /service/businessprocessnotification_businessprocessserver/action/update:
    get:
      summary: Get Service Businessprocessnotification Businessprocessserver Action
        Update
      description: Update an existing Business-Process server object
      operationId: businessProcessServer.update
      x-api-path-slug: servicebusinessprocessnotification-businessprocessserveractionupdate-get
      parameters:
      - in: query
        name: businessProcessServer[dc]
        description: The dc of the server
      - in: query
        name: businessProcessServer[description]
      - in: query
        name: businessProcessServer[host]
      - in: query
        name: businessProcessServer[name]
      - in: query
        name: businessProcessServer[objectType]
      - in: query
        name: businessProcessServer[password]
      - in: query
        name: businessProcessServer[port]
      - in: query
        name: businessProcessServer[protocol]
        description: 'Enum Type: `KalturaActivitiBusinessProcessServerProtocol`'
      - in: query
        name: businessProcessServer[systemName]
      - in: query
        name: businessProcessServer[username]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocessserver
      - Action
      - Update
  /service/caption_captionasset/action/update:
    get:
      summary: Get Service Caption Captionasset Action Update
      description: Update caption asset
      operationId: captionAsset.update
      x-api-path-slug: servicecaption-captionassetactionupdate-get
      parameters:
      - in: query
        name: captionAsset[accuracy]
        description: The Accuracy of the caption content
      - in: query
        name: captionAsset[actualSourceAssetParamsIds]
        description: Comma separated list of source flavor params ids
      - in: query
        name: captionAsset[captionParamsId]
        description: '`insertOnly`The Caption Params used to create this Caption Asset'
      - in: query
        name: captionAsset[fileExt]
        description: '`insertOnly`The file extension'
      - in: query
        name: captionAsset[format]
        description: '`insertOnly`Enum Type: `KalturaCaptionType`The caption format'
      - in: query
        name: captionAsset[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Is default caption asset
          of the entry'
      - in: query
        name: captionAsset[label]
        description: Friendly label
      - in: query
        name: captionAsset[language]
        description: 'Enum Type: `KalturaLanguage`The language of the caption asset
          content'
      - in: query
        name: captionAsset[parentId]
        description: '`insertOnly`The parent id of the asset'
      - in: query
        name: captionAsset[partnerData]
        description: Partner private data
      - in: query
        name: captionAsset[partnerDescription]
        description: Partner friendly description
      - in: query
        name: captionAsset[tags]
        description: Tags used to identify the Flavor Asset in various scenarios
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
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