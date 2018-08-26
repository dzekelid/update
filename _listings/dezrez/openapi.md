---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/agency/updatefee:
    put:
      summary: Add or update fee for logged in agency.
      description: Add or update fee for logged in agency..
      operationId: Agency_UpdateAgencyFeeByfeeDataContract
      x-api-path-slug: apiagencyupdatefee-put
      parameters:
      - in: body
        name: feeDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Update
      - Feelogged
      - In
      - Agency
  /api/amenitydescription/Save:
    post:
      summary: Save or update an Amenity Description
      description: Save or update an amenity description.
      operationId: AmenityDescription_SaveDescriptionByamenityDescriptionDataContract
      x-api-path-slug: apiamenitydescriptionsave-post
      parameters:
      - in: body
        name: amenityDescriptionDataContract
        description: The amenity description to save
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Update
      - Amenity
      - Description
  /api/appointment/saveappointment:
    put:
      summary: Save or update an appointment.
      description: Save or update an appointment..
      operationId: Appointment_SaveAppointmentByappointment
      x-api-path-slug: apiappointmentsaveappointment-put
      parameters:
      - in: body
        name: appointment
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Update
      - Appointment
  /api/auction/saveauction:
    put:
      summary: Save or update an auction.
      description: Save or update an auction..
      operationId: Auction_SaveAuctionByauction
      x-api-path-slug: apiauctionsaveauction-put
      parameters:
      - in: body
        name: auction
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Update
      - Auction
  /api/branch/updatefee:
    put:
      summary: Add or update fee for logged in branch.
      description: Add or update fee for logged in branch..
      operationId: Branch_UpdateBranchFeeByfeeDataContract
      x-api-path-slug: apibranchupdatefee-put
      parameters:
      - in: body
        name: feeDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Update
      - Feelogged
      - In
      - Branch
  /api/chat/message/markasread/{messageId}:
    put:
      summary: This will update the cache with a new timestamp for when this chat
        message was last read.
      description: This will update the cache with a new timestamp for when this chat
        message was last read..
      operationId: Chat_MarkMessageAsReadBymessageId
      x-api-path-slug: apichatmessagemarkasreadmessageid-put
      parameters:
      - in: path
        name: messageId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - This
      - Will
      - Update
      - Cache
      - New
      - Timestampwhen
      - This
      - Chat
      - Message
      - Was
      - Last
      - Read
  /api/Chat:
    put:
      summary: Put - to update a chat message.
      description: Put - to update a chat message..
      operationId: Chat_PutBychatMessageSave
      x-api-path-slug: apichat-put
      parameters:
      - in: body
        name: chatMessageSave
        description: The Appointment JSON object
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - '-'
      - To
      - Update
      - Chat
      - Message
  /api/event/{id}/addnotetoevent:
    post:
      summary: Put - to update a note on an event.
      description: Put - to update a note on an event..
      operationId: Event_AddNoteToEventByidBydataContract
      x-api-path-slug: apieventidaddnotetoevent-post
      parameters:
      - in: body
        name: dataContract
        description: the note text
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the event id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - '-'
      - To
      - Update
      - Note
      - "On"
      - Event
  /api/event/{id}/seteventnote:
    put:
      summary: Put - to update an event note.
      description: Put - to update an event note..
      operationId: Event_UpdateEventNoteByidBynote
      x-api-path-slug: apieventidseteventnote-put
      parameters:
      - in: path
        name: id
        description: the event note id
      - in: query
        name: note
        description: the note text
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - '-'
      - To
      - Update
      - Event
      - Note
  /api/inboundlead/{todoTaskLeadId}/setleadgroup/{groupId}:
    put:
      summary: Endpoint to update group on inbound lead task
      description: Endpoint to update group on inbound lead task.
      operationId: InboundLead_SetLeadGroupBytodoTaskLeadIdBygroupId
      x-api-path-slug: apiinboundleadtodotaskleadidsetleadgroupgroupid-put
      parameters:
      - in: path
        name: groupId
        description: Group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: todoTaskLeadId
        description: Todos Task Id
      responses:
        200:
          description: OK
      tags:
      - Endpoint
      - To
      - Update
      - Group
      - "On"
      - Inbound
      - Lead
      - Task
  /api/localauthoritydescription/Save:
    post:
      summary: Save or update an Local Authority Description
      description: Save or update an local authority description.
      operationId: LocalAuthorityDescription_SaveDescriptionBylocalAuthorityDescriptionDataContract
      x-api-path-slug: apilocalauthoritydescriptionsave-post
      parameters:
      - in: body
        name: localAuthorityDescriptionDataContract
        description: The local authority description to save
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Update
      - Local
      - Authority
      - Description
  /api/region/alias/save:
    post:
      summary: Save or update a region alias
      description: Save or update a region alias.
      operationId: Region_SaveRegionAliasByregionAliasSaveCommand
      x-api-path-slug: apiregionaliassave-post
      parameters:
      - in: body
        name: regionAliasSaveCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Update
      - Region
      - Alias
---