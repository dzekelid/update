---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Discount Update
  description: This method is used to update an existing discount code. Only the fields
    passed as arguments will be modified. This method returns the ID of the modified
    discount code.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /event_update:
    get:
      summary: Get Event Update
      description: This method updates an existing event. Only the fields passed as
        arguments will be modified. This method returns the ID of the modified event.
      operationId: Get_event_update_
      x-api-path-slug: event-update-get
      parameters:
      - in: query
        name: background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_border_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: capacity
        description: The maximum number of people who can attend the event
      - in: query
        name: currency
        description: The event currency in ISO 4217 format (e
      - in: query
        name: custom_footer
        description: Custom HTML footer for your registration page
      - in: query
        name: custom_header
        description: Custom HTML header for your registration page
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The event description
      - in: query
        name: end_date
        description: The event end date and time, in ISO 8601 format (e
      - in: query
        name: event_id
        description: The ID of the event to update
      - in: query
        name: organizer_id
        description: The event organizer ID
      - in: query
        name: personalized_url
        description: The event registration URL subdomain
      - in: query
        name: privacy
        description: 0 for a private event, 1 for a public event
      - in: query
        name: start_date
        description: The event start date and time, in ISO 8601 format (e
      - in: query
        name: status
        description: The event status
      - in: query
        name: text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: timezone
        description: The event time zone in relation to GMT (e
      - in: query
        name: title
        description: The event title
      - in: query
        name: title_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: venue_id
        description: The event venue ID
      responses:
        200:
          description: OK
      tags:
      - Event
      - Update
  /ticket_update:
    get:
      summary: Get Ticket Update
      description: This method updates an existing ticket type. Only the fields passed
        as arguments will be modified. It returns the ID of the updated ticket.
      operationId: Get_ticket_update_
      x-api-path-slug: ticket-update-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The ticket description
      - in: query
        name: end_sales
        description: The date and time when ticket sales stop, in ISO 8601 format
          (e
      - in: query
        name: hide
        description: Show or hide the ticket type
      - in: query
        name: id
        description: The ticket ID
      - in: query
        name: include_fee
        description: 0 to add the Eventbrite service fee on top of ticket price, or
          1 to include it in the ticket price
      - in: query
        name: is_donation
        description: 0 for fixed-price tickets, 1 for donations
      - in: query
        name: max
        description: The maximum number of tickets per order
      - in: query
        name: min
        description: The minimum number of tickets per order
      - in: query
        name: name
        description: The ticket name
      - in: query
        name: price
        description: The ticket price
      - in: query
        name: quantity
        description: The number of tickets available
      - in: query
        name: start_sales
        description: The date and time when ticket sales start, in ISO 8601 format
          (e
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Update
  /venue_update:
    get:
      summary: Get Venue Update
      description: This method updates an existing venue. Only the fields passed as
        arguments will be modified. It returns the ID of the updated venue.
      operationId: Get_venue_update_
      x-api-path-slug: venue-update-get
      parameters:
      - in: query
        name: adress
        description: The venue address (line 1)
      - in: query
        name: adress_2
        description: The venue address (line 2)
      - in: query
        name: city
        description: The venue city
      - in: query
        name: country_code
        description: 2-letter country code, according to the ISO 3166 format
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The venue ID
      - in: query
        name: postal_code
        description: The postal code of the venue
      - in: query
        name: region
        description: The venue state/province/county/territory depending on the country
      - in: query
        name: venue
        description: The venue name
      responses:
        200:
          description: OK
      tags:
      - Venue
      - Update
  /organizer_update:
    get:
      summary: Get Organizer Update
      description: This method updates an existing organizer. Only the fields passed
        as arguments will be modified. It returns the ID of the updated organizer.
      operationId: Get_organizer_update_
      x-api-path-slug: organizer-update-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The organizer description
      - in: query
        name: id
        description: The organizer ID
      - in: query
        name: name
        description: The organizer name
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - Update
  /user_update:
    get:
      summary: Get User Update
      description: This method updates an existing user. Only the fields passed as
        arguments will be modified. It returns the ID of the updated user.
      operationId: Get_user_update_
      x-api-path-slug: user-update-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: new_email
        description: New user email address
      - in: query
        name: new_password
        description: New user password
      responses:
        200:
          description: OK
      tags:
      - User
      - Update
  /discount_update:
    get:
      summary: Get Discount Update
      description: This method is used to update an existing discount code. Only the
        fields passed as arguments will be modified. This method returns the ID of
        the modified discount code.
      operationId: Get_discount_update_
      x-api-path-slug: discount-update-get
      parameters:
      - in: query
        name: amount_off
        description: The fixed amount off the ticket price
      - in: query
        name: code
        description: The discount code
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: end_date
        description: The discount end date and time, in ISO 8601 format (e
      - in: query
        name: id
        description: The discount ID to update
      - in: query
        name: percent_off
        description: The percentage off the ticket price
      - in: query
        name: quantity_available
        description: Maximum number of times this discount can be used
      - in: query
        name: start_date
        description: The discount start date and time, in ISO 8601 format (e
      - in: query
        name: tickets
        description: Comma-separated list of ticket IDs for which the discount applies
      responses:
        200:
          description: OK
      tags:
      - Discount
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