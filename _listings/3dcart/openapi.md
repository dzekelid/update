---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 1
info:
  title: _3dCartWebAPI
  version: 1.0.0
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Cart/{orderkey}:
    put:
      summary: This method is used to update a single cart record in the database.
        The {orderkey} parameter specifies which cart record to update.
      description: This method is used to update a single cart record in the database.
        the {orderkey} parameter specifies which cart record to update..
      operationId: Carts_Update
      x-api-path-slug: 3dcartwebapiv1cartorderkey-put
      parameters:
      - in: body
        name: cart
        description: A Json or XML object containing the cart
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Cart
      - Record
      - In
      - Database
      - ""
      - Orderkey
      - Parameter
      - Specifies
      - Which
      - Cart
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Categories:
    put:
      summary: This method is used to update multiple category records in the database.
        No {categoryid} parameters should be included.
      description: This method is used to update multiple category records in the
        database. no {categoryid} parameters should be included..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categories-put
      parameters:
      - in: body
        name: categories
        description: A Json or XML object containing the new categories
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Category
      - Records
      - In
      - Database
      - ""
      - "No"
      - Categoryid
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Categories/{categoryid}:
    put:
      summary: This method is used to update a single category record in the database.
        The {categoryid} parameter specifies which category to update.
      description: This method is used to update a single category record in the database.
        the {categoryid} parameter specifies which category to update..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryid-put
      parameters:
      - in: body
        name: category
        description: A Json or XML object containing the new category
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryid
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Category
      - Record
      - In
      - Database
      - ""
      - Categoryid
      - Parameter
      - Specifies
      - Which
      - Category
      - To
      - Update
  /3dCartWebAPI/v1/CRM/{id}:
    put:
      summary: This method is used to update a single CRM record in the database.
        The {id} parameter specifies which CRM record to update.
      description: This method is used to update a single crm record in the database.
        the {id} parameter specifies which crm record to update..
      operationId: CRM_UpdateCRM
      x-api-path-slug: 3dcartwebapiv1crmid-put
      parameters:
      - in: body
        name: crm
        description: A Json or XML object containing the new product
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Crm ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - CRM
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/CRM/department/{id}:
    put:
      summary: This method is used to update a single CRM Department record in the
        database. The {id} parameter specifies which CRM Department record to update.
      description: This method is used to update a single crm department record in
        the database. the {id} parameter specifies which crm department record to
        update..
      operationId: CRM_UpdateDepartment
      x-api-path-slug: 3dcartwebapiv1crmdepartmentid-put
      parameters:
      - in: body
        name: department
        description: A Json or XML object containing the new Department
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Department ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - CRM
      - Department
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Department
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/CRM/savedreply/{id}:
    put:
      summary: This method is used to update a single CRM SavedReply record in the
        database. The {id} parameter specifies which CRM SavedReply record to update.
      description: This method is used to update a single crm savedreply record in
        the database. the {id} parameter specifies which crm savedreply record to
        update..
      operationId: CRM_UpdateSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreplyid-put
      parameters:
      - in: path
        name: id
        description: SavedReply ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: savedreply
        description: A Json or XML object containing the new SavedReply
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - CRM
      - SavedReply
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - SavedReply
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/CRM/status/{id}:
    put:
      summary: This method is used to update a single CRM Status record in the database.
        The {id} parameter specifies which CRM Status record to update.
      description: This method is used to update a single crm status record in the
        database. the {id} parameter specifies which crm status record to update..
      operationId: CRM_UpdateStatus
      x-api-path-slug: 3dcartwebapiv1crmstatusid-put
      parameters:
      - in: path
        name: id
        description: Status ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: status
        description: A Json or XML object containing the new Status
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - CRM
      - Status
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Status
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/CustomerGroups/{customergroupid}:
    put:
      summary: This method is used to update a single customer group in the database.
        The {id} parameter specifies which customer group to update.
      description: This method is used to update a single customer group in the database.
        the {id} parameter specifies which customer group to update..
      operationId: CustomerGroups_Update
      x-api-path-slug: 3dcartwebapiv1customergroupscustomergroupid-put
      parameters:
      - in: body
        name: customergroup
        description: A Json or XML object containing the customer group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customergroupid
        description: Customer Group ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Customer
      - Group
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - Customer
      - Group
      - To
      - Update
  /3dCartWebAPI/v1/Customers:
    put:
      summary: This method is used to update multiple customers in the system. No
        URL parameters should be included.
      description: This method is used to update multiple customers in the system.
        no url parameters should be included..
      operationId: Customers_Update
      x-api-path-slug: 3dcartwebapiv1customers-put
      parameters:
      - in: body
        name: customers
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Customers
      - In
      - System
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Customers/{customerid}:
    put:
      summary: This method is used to update a single customer record in the database.
        The {id} parameter specifies which customer record to update.
      description: This method is used to update a single customer record in the database.
        the {id} parameter specifies which customer record to update..
      operationId: Customers_Update
      x-api-path-slug: 3dcartwebapiv1customerscustomerid-put
      parameters:
      - in: body
        name: customer
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerid
        description: Customer ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Customer
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - Customer
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Distributors:
    put:
      summary: This method is used to update multiple distributor records in the database.
        No {distributorid} parameters should be included.
      description: This method is used to update multiple distributor records in the
        database. no {distributorid} parameters should be included..
      operationId: Distributors_Update
      x-api-path-slug: 3dcartwebapiv1distributors-put
      parameters:
      - in: body
        name: distributors
        description: A Json or XML object containing the new distributors
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Distributor
      - Records
      - In
      - Database
      - ""
      - "No"
      - Distributorid
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Distributors/{distributorid}:
    put:
      summary: This method is used to update a single distributor record in the database.
        The {distributorid} parameter specifies which distributor to update.
      description: This method is used to update a single distributor record in the
        database. the {distributorid} parameter specifies which distributor to update..
      operationId: Distributors_Update
      x-api-path-slug: 3dcartwebapiv1distributorsdistributorid-put
      parameters:
      - in: body
        name: distributor
        description: A Json or XML object containing the new distributor
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: distributorid
        description: Distributor ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Distributor
      - Record
      - In
      - Database
      - ""
      - Distributorid
      - Parameter
      - Specifies
      - Which
      - Distributor
      - To
      - Update
  /3dCartWebAPI/v1/Manufacturers:
    put:
      summary: This method is used to update multiple manufacturers in the database.
        No URL parameters should be included.
      description: This method is used to update multiple manufacturers in the database.
        no url parameters should be included..
      operationId: Manufacturer_Update
      x-api-path-slug: 3dcartwebapiv1manufacturers-put
      parameters:
      - in: body
        name: manufacturers
        description: A Json or XML object containing the new manufacturers
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Manufacturers
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Manufacturers/{manufacturerid}:
    put:
      summary: This method is used to update a single manufacturer record in the database.
        The {manufacturerid} parameter specifies which manufacturer record to update.
      description: This method is used to update a single manufacturer record in the
        database. the {manufacturerid} parameter specifies which manufacturer record
        to update..
      operationId: Manufacturer_Update
      x-api-path-slug: 3dcartwebapiv1manufacturersmanufacturerid-put
      parameters:
      - in: body
        name: manufacturer
        description: A Json or XML object containing the new manufacturer
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: manufacturerid
        description: Manufacturer ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Manufacturer
      - Record
      - In
      - Database
      - ""
      - Manufacturerid
      - Parameter
      - Specifies
      - Which
      - Manufacturer
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Orders:
    put:
      summary: This method is used to update multiple orders in the database. No URL
        parameters should be included.
      description: This method is used to update multiple orders in the database.
        no url parameters should be included..
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1orders-put
      parameters:
      - in: body
        name: orders
        description: A Json or XML object containing the orders
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Orders
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Orders/{orderid}:
    put:
      summary: This method is used to update a single order record in the database.
        The {orderid} parameter specifies which order record to update.
      description: This method is used to update a single order record in the database.
        the {orderid} parameter specifies which order record to update..
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderid-put
      parameters:
      - in: body
        name: order
        description: A Json or XML object containing the order
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Order
      - Record
      - In
      - Database
      - ""
      - Orderid
      - Parameter
      - Specifies
      - Which
      - Order
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/PaymentTokens:
    put:
      summary: This method is used to update multiple paymenttokens in the database.
        No URL parameters should be included.
      description: This method is used to update multiple paymenttokens in the database.
        no url parameters should be included..
      operationId: PaymentToken_Update
      x-api-path-slug: 3dcartwebapiv1paymenttokens-put
      parameters:
      - in: body
        name: paymenttokens
        description: A Json or XML object containing the new PaymentTokens
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Paymenttokens
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/PaymentTokens/{paymenttokenid}:
    put:
      summary: This method is used to update a single paymenttoken record in the database.
        The {paymenttokenid} parameter specifies which paymenttoken record to update.
      description: This method is used to update a single paymenttoken record in the
        database. the {paymenttokenid} parameter specifies which paymenttoken record
        to update..
      operationId: PaymentToken_Update
      x-api-path-slug: 3dcartwebapiv1paymenttokenspaymenttokenid-put
      parameters:
      - in: body
        name: paymenttoken
        description: A Json or XML object containing the new paymenttoken
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: paymenttokenid
        description: PaymentTokenID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Paymenttoken
      - Record
      - In
      - Database
      - ""
      - Paymenttokenid
      - Parameter
      - Specifies
      - Which
      - Paymenttoken
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Products:
    put:
      summary: This method is used to update multiple products in the database. No
        URL parameters should be included.
      description: This method is used to update multiple products in the database.
        no url parameters should be included..
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1products-put
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: products
        description: A Json or XML object containing the new product(s)
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Products
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Products/{catalogid}:
    put:
      summary: This method is used to update a single product record in the database.
        The {catalogid} parameter specifies which product record to update.
      description: This method is used to update a single product record in the database.
        the {catalogid} parameter specifies which product record to update..
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: product
        description: A Json or XML object containing the new product
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Product
      - Record
      - In
      - Database
      - ""
      - Catalogid
      - Parameter
      - Specifies
      - Which
      - Product
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/StoreSettings:
    put:
      summary: This method is used to update the Store Settings in the database.
      description: This method is used to update the store settings in the database..
      operationId: StoreSettings_UpdateStoreSettings
      x-api-path-slug: 3dcartwebapiv1storesettings-put
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: settings
        description: A Json or XML object containing the Store Settings
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Store
      - Settings
      - In
      - Database
---