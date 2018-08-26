---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 1
info:
  title: Rebilly
  description: -introductionthe-rebilly-api-is-built-on-http---our-api-is-restful---it-has-predictableresource-urls---it-returns-http-response-codes-to-indicate-errors---it-alsoaccepts-and-returns-json-in-the-http-body---you-can-use-your-favoritehttprest-library-for-your-programming-language-to-use-rebillys-api-oryou-can-use-one-of-our-sdks-currently-available-in-phphttpsgithub-comrebillyrebillyphpand-chttpsgithub-comrebillyrebillydotnetclient--authenticationwhen-you-sign-up-for-an-account-you-are-given-your-first-api-key-you-can-generate-additional-api-keys-and-delete-api-keys-as-you-mayneed-to-rotate-your-keys-in-the-future--you-authenticate-to-therebilly-api-by-providing-your-secret-key-in-the-request-header-rebilly-offers-three-forms-of-authentication--private-key-json-web-tokens-andpublic-key--private-key-authenticates-each-request-by-searching-for-the-presenceof-an-http-header-rebapikey--jwt-authenticates-each-request-by-the-http-header-authorization--public-key-authenticates-by-the-http-header-rebauth-read-more-on-this-below-rebilly-also-offers-json-web-tokens-jwt-authentication-where-you-can-controlthe-specific-granular-permissions-and-expiration-for-that-jwt---we-call-our-resourcefor-generating-jwt-sessionstagsessions-rebilly-also-has-a-clientside-authentication-scheme-that-uses-anapiuser-and-hmacsha1-signature-only-for-the-tokens-resource-sothat-you-may-safely-create-tokens-from-the-clientside-without-compromisingyour-secret-keys-never-share-your-secret-keys--keep-them-guarded-and-secure-the-clientside-authentication-scheme-uses-one-http-header-named-rebauth--redocinject-securitydefinitions--php-sdkfor-all-php-sdk-examples-provided-in-this-spec-you-will-need-to-configure-client-you-may-do-it-like-thisphpclient--new-rebillyclient----apikey--yourapikeyhere----baseurl--httpsapi-rebilly-com
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts/{id}:
    put:
      summary: Create or update a contact with predefined ID
      description: Create or update a contact with predefined identifier string
      operationId: contacts.id.put
      x-api-path-slug: contactsid-put
      parameters:
      - in: body
        name: body
        description: Contact resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Contact
      - Predefined
      - ID
  /coupons/{redemptionCode}:
    put:
      summary: Create or update a coupon with predefined redemption code
      description: Create or update a coupon with predefined redemption code
      operationId: coupons.redemptionCode.put
      x-api-path-slug: couponsredemptioncode-put
      parameters:
      - in: body
        name: body
        description: Coupon resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Coupon
      - Predefined
      - Redemption
      - Code
  /credentials/{id}:
    put:
      summary: Create or update a credential with predefined ID
      description: Create or update a credential with predefined identifier string
      operationId: credentials.id.put
      x-api-path-slug: credentialsid-put
      parameters:
      - in: body
        name: body
        description: Credential resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Credential
      - Predefined
      - ID
  /disputes/{id}:
    put:
      summary: Create or update a Dispute with predefined ID
      description: Create or update a Dispute with predefined identifier string
      operationId: disputes.id.put
      x-api-path-slug: disputesid-put
      parameters:
      - in: body
        name: body
        description: Dispute resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Dispute
      - Predefined
      - ID
  /invoices/{id}:
    put:
      summary: Create or update an invoice with predefined ID
      description: Create or update an invoice with predefined identifier string
      operationId: invoices.id.put
      x-api-path-slug: invoicesid-put
      parameters:
      - in: body
        name: body
        description: Invoice resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Invoice
      - Predefined
      - ID
  /plans/{id}:
    put:
      summary: Create or update a Plan with predefined ID
      description: Create or update a Plan with predefined identifier string
      operationId: plans.id.put
      x-api-path-slug: plansid-put
      parameters:
      - in: body
        name: body
        description: Plan resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Plan
      - Predefined
      - ID
  /subscriptions/{id}:
    put:
      summary: Create or update a subscription with predefined ID
      description: Create or update a subscription with predefined identifier string
      operationId: subscriptions.id.put
      x-api-path-slug: subscriptionsid-put
      parameters:
      - in: body
        name: body
        description: Subscription resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Subscription
      - Predefined
      - ID
  /api-keys/{id}:
    put:
      summary: Create or update api key with predefined ID
      description: Create or update api key with predefined identifier string
      operationId: create-or-update-api-key-with-predefined-identifier-string
      x-api-path-slug: apikeysid-put
      parameters:
      - in: body
        name: body
        description: ApiKey resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Api
      - Key
      - Predefined
      - ID
  /checkout-pages/{id}:
    put:
      summary: Create or update a Checkout Page with predefined ID
      description: Create or update a Checkout Page with predefined identifier string
      operationId: create-or-update-a-checkout-page-with-predefined-identifier-string
      x-api-path-slug: checkoutpagesid-put
      parameters:
      - in: body
        name: body
        description: Checkout Page resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Checkout
      - Page
      - Predefined
      - ID
  /gateway-accounts/{id}:
    put:
      summary: Create or update a Gateway Account with predefined ID
      description: Create or update a GatewayAccount with predefined identifier string
      operationId: create-or-update-a-gatewayaccount-with-predefined-identifier-string
      x-api-path-slug: gatewayaccountsid-put
      parameters:
      - in: body
        name: body
        description: Gateway Account resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Gateway
      - Account
      - Predefined
      - ID
  /layouts/{id}:
    put:
      summary: Create or update a layout with predefined ID
      description: Create or update a layout with predefined identifier string
      operationId: create-or-update-a-layout-with-predefined-identifier-string
      x-api-path-slug: layoutsid-put
      parameters:
      - in: body
        name: body
        description: Layout resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Layout
      - Predefined
      - ID
  /lists/{id}:
    put:
      summary: Create or update a list with predefined ID
      description: Create or update a list with predefined identifier string
      operationId: create-or-update-a-list-with-predefined-identifier-string
      x-api-path-slug: listsid-put
      parameters:
      - in: body
        name: body
        description: List resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - List
      - Predefined
      - ID
  /notes/{id}:
    put:
      summary: Create or update a note with predefined ID
      description: Create or update a note with predefined identifier string
      operationId: create-or-update-a-note-with-predefined-identifier-string
      x-api-path-slug: notesid-put
      parameters:
      - in: body
        name: body
        description: Note resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Note
      - Predefined
      - ID
  /organizations/{id}:
    put:
      summary: Create or update a organization with predefined ID
      description: Create or update a organization with predefined identifier string
      operationId: create-or-update-a-organization-with-predefined-identifier-string
      x-api-path-slug: organizationsid-put
      parameters:
      - in: body
        name: body
        description: Organization resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Organization
      - Predefined
      - ID
  /sessions/{id}:
    put:
      summary: Create or update a Session with predefined ID
      description: Create or update a Session with predefined identifier string
      operationId: create-or-update-a-session-with-predefined-identifier-string
      x-api-path-slug: sessionsid-put
      parameters:
      - in: body
        name: body
        description: Session resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Session
      - Predefined
      - ID
  /users/{id}:
    put:
      summary: Create or update user with predefined ID
      description: Create or update user with predefined identifier string
      operationId: create-or-update-user-with-predefined-identifier-string
      x-api-path-slug: usersid-put
      parameters:
      - in: body
        name: body
        description: User resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - User
      - Predefined
      - ID
  /webhooks/{id}:
    put:
      summary: Create or update a webhook with predefined ID
      description: Create or update a webhook with predefined identifier string
      operationId: create-or-update-a-webhook-with-predefined-identifier-string
      x-api-path-slug: webhooksid-put
      parameters:
      - in: body
        name: body
        description: Webhook resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Webhook
      - Predefined
      - ID
  /websites/{id}:
    put:
      summary: Create or update a website with predefined ID
      description: Create or update a website with predefined identifier string
      operationId: create-or-update-a-website-with-predefined-identifier-string
      x-api-path-slug: websitesid-put
      parameters:
      - in: body
        name: body
        description: Website resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Website
      - Predefined
      - ID
  /websites/{id}/webhook:
    put:
      summary: Create or update a webhook for website with predefined ID
      description: Create or update a webhook for website with predefined identifier
        string
      operationId: create-or-update-a-webhook-for-website-with-predefined-identifier-string
      x-api-path-slug: websitesidwebhook-put
      parameters:
      - in: body
        name: body
        description: Webhook resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Webhookwebsite
      - Predefined
      - ID
---