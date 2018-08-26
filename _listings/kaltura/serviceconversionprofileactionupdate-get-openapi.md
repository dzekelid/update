---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Conversionprofile Action Update
  description: Update Conversion Profile by ID
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
  /service/caption_captionparams/action/update:
    get:
      summary: Get Service Caption Captionparams Action Update
      description: Update Caption Params by ID
      operationId: captionParams.update
      x-api-path-slug: servicecaption-captionparamsactionupdate-get
      parameters:
      - in: query
        name: captionParams[description]
        description: The description of the Flavor Params
      - in: query
        name: captionParams[format]
        description: '`insertOnly`Enum Type: `KalturaCaptionType`The caption format'
      - in: query
        name: captionParams[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Is default caption asset
          of the entry'
      - in: query
        name: captionParams[label]
        description: Friendly label
      - in: query
        name: captionParams[language]
        description: '`insertOnly`Enum Type: `KalturaLanguage`The language of the
          caption content'
      - in: query
        name: captionParams[mediaParserType]
        description: 'Enum Type: `KalturaMediaParserType`Media parser type to be used
          for post-conversion validation'
      - in: query
        name: captionParams[name]
        description: The name of the Flavor Params
      - in: query
        name: captionParams[partnerId]
      - in: query
        name: captionParams[remoteStorageProfileIds]
        description: Comma seperated ids of remote storage profiles that the flavor
          distributed to, the distribution done by the conversion engine
      - in: query
        name: captionParams[requiredPermissions]
      - in: query
        name: captionParams[sourceAssetParamsIds]
        description: Comma seperated ids of source flavor params this flavor is created
          from
      - in: query
        name: captionParams[sourceParamsId]
        description: Id of the caption params or the flavor params to be used as source
          for the caption creation
      - in: query
        name: captionParams[sourceRemoteStorageProfileId]
        description: Id of remote storage profile that used to get the source, zero
          indicates Kaltura data center
      - in: query
        name: captionParams[systemName]
        description: System name of the Flavor Params
      - in: query
        name: captionParams[tags]
        description: The Flavor Params tags are used to identify the flavor for different
          usage (e
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
      - Captionparams
      - Action
      - Update
  /service/category/action/update:
    get:
      summary: Get Service Category Action Update
      description: Update Category
      operationId: category.update
      x-api-path-slug: servicecategoryactionupdate-get
      parameters:
      - in: query
        name: category[aggregationCategories]
        description: List of aggregation channels the category belongs to
      - in: query
        name: category[appearInList]
        description: 'Enum Type: `KalturaAppearInListType`If category will be returned
          for list action'
      - in: query
        name: category[contributionPolicy]
        description: 'Enum Type: `KalturaContributionPolicyType`who can assign entries
          to this category'
      - in: query
        name: category[defaultOrderBy]
        description: 'Enum Type: `KalturaCategoryOrderBy`Enable client side applications
          to define how to sort the category child categories'
      - in: query
        name: category[defaultPermissionLevel]
        description: 'Enum Type: `KalturaCategoryUserPermissionLevel`Default permissionLevel
          for new users'
      - in: query
        name: category[description]
        description: Category description
      - in: query
        name: category[inheritanceType]
        description: 'Enum Type: `KalturaInheritanceType`If Category members are inherited
          from parent category or set manualy'
      - in: query
        name: category[isAggregationCategory]
        description: 'Enum Type: `KalturaNullableBoolean`Flag indicating that the
          category is an aggregation category'
      - in: query
        name: category[moderation]
        description: 'Enum Type: `KalturaNullableBoolean`Moderation to add entries
          to this category by users that are not of permission level Manager or Moderator'
      - in: query
        name: category[name]
        description: The name of the Category
      - in: query
        name: category[owner]
        description: Category Owner (User id)
      - in: query
        name: category[parentId]
      - in: query
        name: category[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: category[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: category[privacyContext]
        description: Set privacy context for search entries that assiged to private
          and public categories
      - in: query
        name: category[privacy]
        description: 'Enum Type: `KalturaPrivacyType`defines the privacy of the entries
          that assigned to this category'
      - in: query
        name: category[referenceId]
        description: Category external id, controlled and managed by the partner
      - in: query
        name: category[tags]
        description: Category tags
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Update
  /service/categoryuser/action/update:
    get:
      summary: Get Service Categoryuser Action Update
      description: Update CategoryUser by id
      operationId: categoryUser.update
      x-api-path-slug: servicecategoryuseractionupdate-get
      parameters:
      - in: query
        name: categoryId
      - in: query
        name: categoryUser[categoryId]
        description: '`insertOnly`'
      - in: query
        name: categoryUser[permissionLevel]
        description: 'Enum Type: `KalturaCategoryUserPermissionLevel`Permission level'
      - in: query
        name: categoryUser[permissionNames]
        description: Set of category-related permissions for the current category
          user
      - in: query
        name: categoryUser[updateMethod]
        description: 'Enum Type: `KalturaUpdateMethodType`Update method can be either
          manual or automatic to distinguish between manual operations (for example
          in KMC) on automatic - using bulk upload'
      - in: query
        name: categoryUser[userId]
        description: '`insertOnly`User id'
      - in: query
        name: No Name
      - in: query
        name: override
        description: '- to override manual changes'
      - in: query
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Categoryuser
      - Action
      - Update
  /service/contentdistribution_distributionprofile/action/update:
    get:
      summary: Get Service Contentdistribution Distributionprofile Action Update
      description: Update Distribution Profile by id
      operationId: distributionProfile.update
      x-api-path-slug: servicecontentdistribution-distributionprofileactionupdate-get
      parameters:
      - in: query
        name: distributionProfile[accountId]
      - in: query
        name: distributionProfile[adFreeApplicationGuid]
        description: The GUID for the application in which to record metrics and enforce
          business rules obtained through your Unicorn representative
      - in: query
        name: distributionProfile[adServerPartnerId]
      - in: query
        name: distributionProfile[allowAdsenseForVideo]
      - in: query
        name: distributionProfile[allowComments]
      - in: query
        name: distributionProfile[allowDownload]
      - in: query
        name: distributionProfile[allowEmbedding]
      - in: query
        name: distributionProfile[allowInvideo]
      - in: query
        name: distributionProfile[allowMidRollAds]
      - in: query
        name: distributionProfile[allowPostRollAds]
      - in: query
        name: distributionProfile[allowPreRollAds]
      - in: query
        name: distributionProfile[allowRatings]
      - in: query
        name: distributionProfile[allowResponses]
      - in: query
        name: distributionProfile[allowStreaming]
      - in: query
        name: distributionProfile[allowSyndication]
      - in: query
        name: distributionProfile[apiAuthorizeUrl]
      - in: query
        name: distributionProfile[apiHostUrl]
        description: The API host URL that the Upload User should have access to,
          Used for HTTP content submission
      - in: query
        name: distributionProfile[apikey]
      - in: query
        name: distributionProfile[asperaHost]
      - in: query
        name: distributionProfile[asperaLogin]
      - in: query
        name: distributionProfile[asperaPass]
      - in: query
        name: distributionProfile[asperaPrivateKey]
      - in: query
        name: distributionProfile[asperaPublicKey]
      - in: query
        name: distributionProfile[assetFilenameXslt]
      - in: query
        name: distributionProfile[assumeSuccess]
      - in: query
        name: distributionProfile[autoCreateFlavors]
        description: Comma separated flavor params ids that should be auto converted
      - in: query
        name: distributionProfile[autoCreateThumb]
        description: Comma separated thumbnail params ids that should be auto generated
      - in: query
        name: distributionProfile[backgroundImageStandard]
      - in: query
        name: distributionProfile[backgroundImageWide]
      - in: query
        name: distributionProfile[basePath]
      - in: query
        name: distributionProfile[blockOutsideOwnership]
      - in: query
        name: distributionProfile[bodyXslt]
      - in: query
        name: distributionProfile[captionAutosync]
      - in: query
        name: distributionProfile[categoryId]
      - in: query
        name: distributionProfile[certificateKey]
      - in: query
        name: distributionProfile[channelCopyright]
      - in: query
        name: distributionProfile[channelDescription]
      - in: query
        name: distributionProfile[channelGenerator]
      - in: query
        name: distributionProfile[channelGuid]
        description: The Channel GUID assigned to this Publication Rule
      - in: query
        name: distributionProfile[channelImageHeight]
      - in: query
        name: distributionProfile[channelImageLink]
      - in: query
        name: distributionProfile[channelImageTitle]
      - in: query
        name: distributionProfile[channelImageUrl]
      - in: query
        name: distributionProfile[channelImageWidth]
      - in: query
        name: distributionProfile[channelLanguage]
      - in: query
        name: distributionProfile[channelLink]
      - in: query
        name: distributionProfile[channelManagingEditor]
      - in: query
        name: distributionProfile[channelRating]
      - in: query
        name: distributionProfile[channelTitle]
      - in: query
        name: distributionProfile[claimType]
      - in: query
        name: distributionProfile[commercialPolicy]
      - in: query
        name: distributionProfile[contactEmail]
      - in: query
        name: distributionProfile[contactTelephone]
      - in: query
        name: distributionProfile[contentOwner]
      - in: query
        name: distributionProfile[copyright]
      - in: query
        name: distributionProfile[cPlatformTvSeriesField]
      - in: query
        name: distributionProfile[cPlatformTvSeries]
      - in: query
        name: distributionProfile[csId]
      - in: query
        name: distributionProfile[cuePointsProvider]
      - in: query
        name: distributionProfile[defaultCategory]
      - in: query
        name: distributionProfile[deleteEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: distributionProfile[deleteReference]
      - in: query
        name: distributionProfile[disableEpisodeNumberCustomValidation]
      - in: query
        name: distributionProfile[disableMetadata]
      - in: query
        name: distributionProfile[distributeCaptions]
      - in: query
        name: distributionProfile[distributeCuePoints]
      - in: query
        name: distributionProfile[distributeRemoteCaptionAssetContent]
      - in: query
        name: distributionProfile[distributeRemoteFlavorAssetContent]
      - in: query
        name: distributionProfile[distributeRemoteThumbAssetContent]
      - in: query
        name: distributionProfile[domainGuid]
        description: The GUID of the Customer Domain in the Unicorn system obtained
          by contacting your Unicorn representative
      - in: query
        name: distributionProfile[domainName]
        description: The name of the Domain that the Upload User should have access
          to, Used for authentication
      - in: query
        name: distributionProfile[domain]
      - in: query
        name: distributionProfile[downloadPriceCode]
      - in: query
        name: distributionProfile[email]
      - in: query
        name: distributionProfile[enableAdServer]
      - in: query
        name: distributionProfile[entitlements]
      - in: query
        name: distributionProfile[entitlement]
      - in: query
        name: distributionProfile[feedAuthorName]
      - in: query
        name: distributionProfile[feedCopyright]
      - in: query
        name: distributionProfile[feedDescription]
      - in: query
        name: distributionProfile[feedImageHeight]
      - in: query
        name: distributionProfile[feedImageLink]
      - in: query
        name: distributionProfile[feedImageTitle]
      - in: query
        name: distributionProfile[feedImageUrl]
      - in: query
        name: distributionProfile[feedImageWidth]
      - in: query
        name: distributionProfile[feedLanguage]
      - in: query
        name: distributionProfile[feedLastBuildDate]
      - in: query
        name: distributionProfile[feedLink]
      - in: query
        name: distributionProfile[feedSpecVersion]
        description: 'Enum Type: `KalturaYouTubeDistributionFeedSpecVersion`'
      - in: query
        name: distributionProfile[feedSubtitle]
      - in: query
        name: distributionProfile[feedTitle]
      - in: query
        name: distributionProfile[fieldConfigArray]
      - in: query
        name: distributionProfile[flavorAssetFilenameXslt]
      - in: query
        name: distributionProfile[flvFlavorParamsId]
      - in: query
        name: distributionProfile[ftpHost]
      - in: query
        name: distributionProfile[ftpLogin]
      - in: query
        name: distributionProfile[ftpPassword]
      - in: query
        name: distributionProfile[ftpPass]
      - in: query
        name: distributionProfile[ftpPath]
      - in: query
        name: distributionProfile[ftpUsername]
      - in: query
        name: distributionProfile[genericProviderId]
        description: '`insertOnly`'
      - in: query
        name: distributionProfile[geoBlockingMapping]
        description: 'Enum Type: `KalturaDailymotionGeoBlockingMapping`'
      - in: query
        name: distributionProfile[googleClientId]
      - in: query
        name: distributionProfile[googleClientSecret]
      - in: query
        name: distributionProfile[googleTokenData]
      - in: query
        name: distributionProfile[hideViewCount]
      - in: query
        name: distributionProfile[host]
      - in: query
        name: distributionProfile[ignoreSchedulingInFeed]
      - in: query
        name: distributionProfile[ingestUrl]
      - in: query
        name: distributionProfile[instreamStandard]
      - in: query
        name: distributionProfile[instreamTrueview]
      - in: query
        name: distributionProfile[ips]
      - in: query
        name: distributionProfile[itemLink]
      - in: query
        name: distributionProfile[itemMediaRating]
      - in: query
        name: distributionProfile[itemsPerPage]
      - in: query
        name: distributionProfile[itemType]
      - in: query
        name: distributionProfile[itemXpathsToExtend]
      - in: query
        name: distributionProfile[mapAccessControlProfileIds]
      - in: query
        name: distributionProfile[mapCaptionParamsIds]
      - in: query
        name: distributionProfile[mapConversionProfileIds]
      - in: query
        name: distributionProfile[mapFlavorParamsIds]
      - in: query
        name: distributionProfile[mapMetadataProfileIds]
      - in: query
        name: distributionProfile[mapStorageProfileIds]
      - in: query
        name: distributionProfile[mapThumbParamsIds]
      - in: query
        name: distributionProfile[metadataFilenameXslt]
      - in: query
        name: distributionProfile[metadataProfileId]
      - in: query
        name: distributionProfile[metadataXpathsTriggerUpdate]
      - in: query
        name: distributionProfile[metadataXslt]
      - in: query
        name: distributionProfile[msnvideoCat]
      - in: query
        name: distributionProfile[msnvideoTopCat]
      - in: query
        name: distributionProfile[msnvideoTop]
      - in: query
        name: distributionProfile[name]
      - in: query
        name: distributionProfile[notificationEmail]
      - in: query
        name: distributionProfile[objectType]
      - in: query
        name: distributionProfile[optionalAssetDistributionRules]
      - in: query
        name: distributionProfile[optionalFlavorParamsIds]
        description: Comma separated flavor params ids that should be submitted if
          ready
      - in: query
        name: distributionProfile[optionalThumbDimensions]
      - in: query
        name: distributionProfile[overrideManualEdits]
      - in: query
        name: distributionProfile[ownerName]
      - in: query
        name: distributionProfile[pageAccessToken]
      - in: query
        name: distributionProfile[pageGroup]
      - in: query
        name: distributionProfile[pageId]
      - in: query
        name: distributionProfile[passphrase]
      - in: query
        name: distributionProfile[password]
      - in: query
        name: distributionProfile[permissions]
      - in: query
        name: distributionProfile[port]
      - in: query
        name: distributionProfile[priority]
      - in: query
        name: distributionProfile[privacyStatus]
      - in: query
        name: distributionProfile[processFeed]
        description: 'Enum Type: `KalturaYahooDistributionProcessFeedActionStatus`'
      - in: query
        name: distributionProfile[protocol]
        description: '`insertOnly`Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: distributionProfile[providerId]
      - in: query
        name: distributionProfile[providerName]
      - in: query
        name: distributionProfile[providerType]
        description: '`insertOnly`Enum Type: `KalturaDistributionProviderType`'
      - in: query
        name: distributionProfile[rating]
      - in: query
        name: distributionProfile[recommendedDcForDownload]
        description: The best Kaltura data center to be used to download the asset
          files to
      - in: query
        name: distributionProfile[recommendedDcForExecute]
        description: The best Kaltura data center to be used to execute the distribution
          job
      - in: query
        name: distributionProfile[recommendedStorageProfileForDownload]
        description: The best external storage to be used to download the asset files
          from
      - in: query
        name: distributionProfile[releaseClaims]
      - in: query
        name: distributionProfile[remoteAssetParamsId]
        description: The flavor-params that will be used for the remote asset
      - in: query
        name: distributionProfile[replaceAirDates]
      - in: query
        name: distributionProfile[replaceGroup]
      - in: query
        name: distributionProfile[reportEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: distributionProfile[requiredAssetDistributionRules]
      - in: query
        name: distributionProfile[requiredFlavorParamsIds]
        description: Comma separated flavor params ids that required to be ready before
          submission
      - in: query
        name: distributionProfile[requiredThumbDimensions]
      - in: query
        name: distributionProfile[reRequestPermissions]
      - in: query
        name: distributionProfile[seasonNumber]
      - in: query
        name: distributionProfile[seasonSynopsis]
      - in: query
        name: distributionProfile[seasonTuneInInformation]
      - in: query
        name: distributionProfile[sendMetadataAfterAssets]
      - in: query
        name: distributionProfile[seriesAdditionalCategories]
      - in: query
        name: distributionProfile[seriesChannel]
      - in: query
        name: distributionProfile[seriesPrimaryCategory]
      - in: query
        name: distributionProfile[sftpBaseDir]
      - in: query
        name: distributionProfile[sftpBasePath]
      - in: query
        name: distributionProfile[sftpHost]
      - in: query
        name: distributionProfile[sftpLogin]
      - in: query
        name: distributionProfile[sftpPass]
      - in: query
        name: distributionProfile[sftpPort]
      - in: query
        name: distributionProfile[sftpPrivateKey]
      - in: query
        name: distributionProfile[sftpPublicKey]
      - in: query
        name: distributionProfile[shouldAddThumbExtension]
      - in: query
        name: distributionProfile[shouldIncludeCaptions]
      - in: query
        name: distributionProfile[shouldIncludeCuePoints]
      - in: query
        name: distributionProfile[slFlavorParamsId]
      - in: query
        name: distributionProfile[slHdFlavorParamsId]
      - in: query
        name: distributionProfile[sourceFlavorParamsId]
      - in: query
        name: distributionProfile[sourceFriendlyName]
      - in: query
        name: distributionProfile[source]
      - in: query
        name: distributionProfile[state]
      - in: query
        name: distributionProfile[status]
        description: 'Enum Type: `KalturaDistributionProfileStatus`'
      - in: query
        name: distributionProfile[storageProfileId]
        description: The remote storage that should be used for the remote asset
      - in: query
        name: distributionProfile[streamingPriceCode]
      - in: query
        name: distributionProfile[strict]
      - in: query
        name: distributionProfile[submitAction][ftpPassiveMode]
      - in: query
        name: distributionProfile[submitAction][httpFieldName]
      - in: query
        name: distributionProfile[submitAction][httpFileName]
      - in: query
        name: distributionProfile[submitAction][password]
      - in: query
        name: distributionProfile[submitAction][protocol]
        description: 'Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: distributionProfile[submitAction][serverPath]
      - in: query
        name: distributionProfile[submitAction][serverUrl]
      - in: query
        name: distributionProfile[submitAction][username]
      - in: query
        name: distributionProfile[submitEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: distributionProfile[sunriseDefaultOffset]
        description: If entry distribution sunrise not specified that will be the
          default since entry creation time, in seconds
      - in: query
        name: distributionProfile[sunsetDefaultOffset]
        description: If entry distribution sunset not specified that will be the default
          since entry creation time, in seconds
      - in: query
        name: distributionProfile[tags]
      - in: query
        name: distributionProfile[targetAccountId]
      - in: query
        name: distributionProfile[targetLoginId]
      - in: query
        name: distributionProfile[targetLoginPassword]
      - in: query
        name: distributionProfile[targetServiceUrl]
      - in: query
        name: distributionProfile[target]
      - in: query
        name: distributionProfile[thumbnailAssetFilenameXslt]
      - in: query
        name: distributionProfile[ugcPolicy]
      - in: query
        name: distributionProfile[updateEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: distributionProfile[upstreamNetworkId]
      - in: query
        name: distributionProfile[upstreamNetworkName]
      - in: query
        name: distributionProfile[upstreamVideoId]
      - in: query
        name: distributionProfile[urgentReference]
      - in: query
        name: distributionProfile[useCategoryEntries]
        description: When checking custom XSLT conditions using the fieldConfigArray
          - address only categories associated with the entry via the categoryEntry
          object
      - in: query
        name: distributionProfile[userAccessToken]
      - in: query
        name: distributionProfile[username]
      - in: query
        name: distributionProfile[user]
      - in: query
        name: distributionProfile[videoMediaType]
      - in: query
        name: distributionProfile[wmvFlavorParamsId]
      - in: query
        name: distributionProfile[xsltFile]
      - in: query
        name: distributionProfile[xsl]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Distributionprofile
      - Action
      - Update
  /service/contentdistribution_entrydistribution/action/update:
    get:
      summary: Get Service Contentdistribution Entrydistribution Action Update
      description: Update Entry Distribution by id
      operationId: entryDistribution.update
      x-api-path-slug: servicecontentdistribution-entrydistributionactionupdate-get
      parameters:
      - in: query
        name: entryDistribution[assetIds]
        description: Comma separated asset ids
      - in: query
        name: entryDistribution[distributionProfileId]
        description: '`insertOnly`'
      - in: query
        name: entryDistribution[entryId]
        description: '`insertOnly`'
      - in: query
        name: entryDistribution[flavorAssetIds]
        description: Comma separated flavor asset ids
      - in: query
        name: entryDistribution[sunrise]
        description: Entry distribution publish time as Unix timestamp (In seconds)
      - in: query
        name: entryDistribution[sunset]
        description: Entry distribution un-publish time as Unix timestamp (In seconds)
      - in: query
        name: entryDistribution[thumbAssetIds]
        description: Comma separated thumbnail asset ids
      - in: query
        name: entryDistribution[validationErrors]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Entrydistribution
      - Action
      - Update
  /service/contentdistribution_genericdistributionprovider/action/update:
    get:
      summary: Get Service Contentdistribution Genericdistributionprover Action Update
      description: Update Generic Distribution Provider by id
      operationId: genericDistributionProvider.update
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionupdate-get
      parameters:
      - in: query
        name: genericDistributionProvider[availabilityUpdateEnabled]
      - in: query
        name: genericDistributionProvider[deleteInsteadUpdate]
      - in: query
        name: genericDistributionProvider[editableFields]
      - in: query
        name: genericDistributionProvider[intervalBeforeSunrise]
      - in: query
        name: genericDistributionProvider[intervalBeforeSunset]
      - in: query
        name: genericDistributionProvider[isDefault]
      - in: query
        name: genericDistributionProvider[mandatoryFields]
      - in: query
        name: genericDistributionProvider[name]
      - in: query
        name: genericDistributionProvider[optionalFlavorParamsIds]
      - in: query
        name: genericDistributionProvider[optionalThumbDimensions]
      - in: query
        name: genericDistributionProvider[requiredFlavorParamsIds]
      - in: query
        name: genericDistributionProvider[requiredThumbDimensions]
      - in: query
        name: genericDistributionProvider[scheduleUpdateEnabled]
      - in: query
        name: genericDistributionProvider[updateRequiredEntryFields]
      - in: query
        name: genericDistributionProvider[updateRequiredMetadataXPaths]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovider
      - Action
      - Update
  /service/contentdistribution_genericdistributionprovideraction/action/update:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Update
      description: Update Generic Distribution Provider Action by id
      operationId: genericDistributionProviderAction.update
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionupdate-get
      parameters:
      - in: query
        name: genericDistributionProviderAction[action]
        description: '`insertOnly`Enum Type: `KalturaDistributionAction`'
      - in: query
        name: genericDistributionProviderAction[editableFields]
      - in: query
        name: genericDistributionProviderAction[genericDistributionProviderId]
        description: '`insertOnly`'
      - in: query
        name: genericDistributionProviderAction[mandatoryFields]
      - in: query
        name: genericDistributionProviderAction[protocol]
        description: 'Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: genericDistributionProviderAction[remotePassword]
      - in: query
        name: genericDistributionProviderAction[remotePath]
      - in: query
        name: genericDistributionProviderAction[remoteUsername]
      - in: query
        name: genericDistributionProviderAction[resultsParser]
        description: 'Enum Type: `KalturaGenericDistributionProviderParser`'
      - in: query
        name: genericDistributionProviderAction[serverAddress]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - Update
  /service/conversionprofile/action/update:
    get:
      summary: Get Service Conversionprofile Action Update
      description: Update Conversion Profile by ID
      operationId: conversionProfile.update
      x-api-path-slug: serviceconversionprofileactionupdate-get
      parameters:
      - in: query
        name: conversionProfile[cropDimensions][height]
        description: Crop height
      - in: query
        name: conversionProfile[cropDimensions][left]
        description: Crop left point
      - in: query
        name: conversionProfile[cropDimensions][top]
        description: Crop top point
      - in: query
        name: conversionProfile[cropDimensions][width]
        description: Crop width
      - in: query
        name: conversionProfile[defaultEntryId]
        description: ID of the default entry to be used for template data
      - in: query
        name: conversionProfile[description]
        description: The description of the Conversion Profile
      - in: query
        name: conversionProfile[flavorParamsIds]
        description: List of included flavor ids (comma separated)
      - in: query
        name: conversionProfile[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that this conversion
          profile is system default'
      - in: query
        name: conversionProfile[name]
        description: The name of the Conversion Profile
      - in: query
        name: conversionProfile[status]
        description: 'Enum Type: `KalturaConversionProfileStatus`'
      - in: query
        name: conversionProfile[systemName]
        description: System name of the Conversion Profile
      - in: query
        name: conversionProfile[tags]
        description: Comma separated tags
      - in: query
        name: conversionProfile[type]
        description: '`insertOnly`Enum Type: `KalturaConversionProfileType`'
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofile
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