{
  "info": {
    "name": "Eventbrite Get Discount Update",
    "_postman_id": "ad22dbe1-6301-43dd-a16a-2e85728e902e",
    "description": "This method is used to update an existing discount code. Only the fields passed as arguments will be modified. This method returns the ID of the modified discount code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Checkout",
      "item": [
        {
          "id": "04aa4cfe-e72a-43f2-843b-2e00719d8972",
          "name": "getCheckoutSettingsCountriesCurrencies",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/checkout_settings/countries_currencies/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the countries and currencies which are supported by Eventbrite for ticket payment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "145cae92-b563-4900-882b-6cb2677d5539"
            }
          ]
        }
      ]
    },
    {
      "name": "Discounts",
      "item": [
        {
          "id": "6697c19c-a791-4b8b-87b4-05bf4bf10ad7",
          "name": "getDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the cross_event_discount with the specified :discount_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "055eb8f6-e4df-44f2-959d-832cee492710"
            }
          ]
        },
        {
          "id": "837f816b-805d-4d49-b3b8-0b544e448da7",
          "name": "postDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/?discount.amount_off=%7B%7D&discount.code=%7B%7D&discount.end_date=%7B%7D&discount.end_date_relative=%7B%7D&discount.hold_ids=%7B%7D&discount.percent_off=%7B%7D&discount.quantity_available=%7B%7D&discount.start_date=%7B%7D&discount.start_date_relative=%7B%7D&discount.ticket_class_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the discount with the specified :discount_id. Returns the updated cross_event_discount. The fields sent are the ones that are going to be updated, the fields that are not sent will be unchanged. The same conditions and notes for the discount creation apply."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e048720-744f-4933-94eb-5098d5b60dde"
            }
          ]
        },
        {
          "id": "05e79ad9-b0bc-4d9a-b317-021192d47858",
          "name": "deleteDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the cross_event_discount with the specified :discount_id.\nOnly unused discounts can be deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "738a6a2a-de3f-463b-947d-9d45995fca2b"
            }
          ]
        },
        {
          "id": "e4d8d546-6c77-461e-b199-448a60bee88e",
          "name": "postDiscounts",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/?discount.amount_off=%7B%7D&discount.code=%7B%7D&discount.end_date=%7B%7D&discount.end_date_relative=%7B%7D&discount.event_id=%7B%7D&discount.hold_ids=%7B%7D&discount.percent_off=%7B%7D&discount.quantity_available=%7B%7D&discount.start_date=%7B%7D&discount.start_date_relative=%7B%7D&discount.ticket_class_ids=%7B%7D&discount.ticket_group_id=%7B%7D&discount.type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a discount. Returns the created cross_event_discount."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dd9e67e-5215-4d72-bab3-71728d6e2600"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "5260de51-c543-401b-ba45-6522944d5f37",
          "name": "getEventsDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f310c44-9d9f-4b4e-96b5-59fae6991475"
            }
          ]
        },
        {
          "id": "3c650c9c-2c7e-4215-8e07-453738c4c054",
          "name": "postEventsDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "102be8b4-15cf-4ac9-9c0b-2ab66529a162"
            }
          ]
        },
        {
          "id": "58e2a581-da46-43ec-9d05-66f09ea404f4",
          "name": "getEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ebd86bf-25ab-4e0a-b71d-867e6fc3092d"
            }
          ]
        },
        {
          "id": "d1e5c1a6-095b-41f2-83b5-aead9854d8a2",
          "name": "postEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2376432d-9741-4097-a301-1fc07d032e04"
            }
          ]
        },
        {
          "id": "d1880e72-23f3-463b-8044-349ec7a420b7",
          "name": "deleteEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6745d0d5-dfd2-4b30-9a29-efd131a7798c"
            }
          ]
        },
        {
          "id": "460d8f1f-d463-4f5e-8513-0f9b2b22d1a8",
          "name": "getEventsPublicDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5c5fc0a-6e34-4155-b5fd-4b6be340443c"
            }
          ]
        },
        {
          "id": "7c892558-da43-41e1-b13e-2e5baa20fdfe",
          "name": "postEventsPublicDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9d23225-014b-480a-8a59-35132a601a6f"
            }
          ]
        },
        {
          "id": "06479718-05e1-4e39-a2ea-f23153e59afd",
          "name": "getEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0aeda21-899c-4a94-92c6-1640eef9550d"
            }
          ]
        },
        {
          "id": "321e0a45-194d-4840-84d6-232988a6645f",
          "name": "postEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89e897c1-81e3-4ec2-a2a3-c34ff964e5d2"
            }
          ]
        },
        {
          "id": "e3e65b28-9f5e-45f6-ac5e-7719174886a8",
          "name": "deleteEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e4fed25-d086-4a14-b523-fba4faa44296"
            }
          ]
        }
      ]
    },
    {
      "name": "System",
      "item": [
        {
          "id": "a75ce0d7-6dc8-4cb0-8fc2-8e3f7a049ccc",
          "name": "getSystemCountries",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/system/countries/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single page response with a key of countries,\ncontaining a list of countries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ee36037-53e8-4443-a528-1e27a8b913cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "f5c87539-0301-4696-8688-4bdf4976a49a",
          "name": "getUsersUserDiscounts",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/users/:user_id/discounts/?code=%7B%7D&code_filter=%7B%7D&event_id=%7B%7D&order_by=%7B%7D&page_size=%7B%7D&scope=%7B%7D&ticket_group_id=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated response of cross_event_discount for the specified user.\nThis operation is only supported for the currently authenticated user. The alias me (/users/me/) may be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b00a45c1-ecff-45bd-b1d2-3809c520d77a"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "245864fe-a6cc-44ec-bf0e-f54cf71a3423",
          "name": "Get_event_list_discounts_",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/event_list_discounts?data-type=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method returns a list of discounts for a given event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad0a543e-1949-4b9a-bf68-357927f4c93f"
            }
          ]
        }
      ]
    },
    {
      "name": "Discount",
      "item": [
        {
          "id": "096d8f26-ce41-48c0-b4b9-6abf1995dbdc",
          "name": "Get_discount_new_",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discount_new?amount_off=%7B%7D&code=%7B%7D&data-type=%7B%7D&end_date=%7B%7D&event_id=%7B%7D&percent_off=%7B%7D&quantity_available=%7B%7D&start_date=%7B%7D&tickets=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method creates a new discount code for a specific event. It returns the ID of the newly created discount code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f11502d-2fe4-43ef-bee0-7f1e90603d83"
            }
          ]
        },
        {
          "id": "01c411f2-0a75-4a45-a8c6-37242bea4536",
          "name": "Get_discount_update_",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discount_update?amount_off=%7B%7D&code=%7B%7D&data-type=%7B%7D&end_date=%7B%7D&id=%7B%7D&percent_off=%7B%7D&quantity_available=%7B%7D&start_date=%7B%7D&tickets=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method is used to update an existing discount code. Only the fields passed as arguments will be modified. This method returns the ID of the modified discount code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dce5349-98de-4f3d-8b33-6f52fa233c8d"
            }
          ]
        }
      ]
    }
  ]
}