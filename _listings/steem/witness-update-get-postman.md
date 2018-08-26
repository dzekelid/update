{
  "info": {
    "name": "Steem witness_update",
    "_postman_id": "35573d14-7479-4e66-8912-4bf4114a8c69",
    "description": "witness_update",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "60a4bbb0-b0da-4cd1-87bb-ffee91d1a640",
          "name": "get-witnesses",
          "request": {
            "url": "http://api.steemjs.com/get_witnesses?witnessIds=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_witnesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ed4f736-650c-4eaa-9476-e60cc6cc29ab"
            }
          ]
        },
        {
          "id": "36ca1719-a46c-42a1-92f0-5c65fb19a452",
          "name": "get-witnesses-by-vote",
          "request": {
            "url": "http://api.steemjs.com/get_witnesses_by_vote?from=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_witnesses_by_vote"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49a985ed-d778-4ed0-84d7-e85842005b70"
            }
          ]
        },
        {
          "id": "58e6f3b5-8dbc-4ed4-bbe6-d4b386823ff0",
          "name": "get-active-witnesses",
          "request": {
            "url": "http://api.steemjs.com/get_active_witnesses",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_active_witnesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c79118cb-50e3-47c6-9ce5-773f0ff93596"
            }
          ]
        },
        {
          "id": "a36c2f00-f4c8-4c1f-b231-146d30a7dc27",
          "name": "get-witness-count",
          "request": {
            "url": "http://api.steemjs.com/get_witness_count",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_witness_count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b83b5903-f806-4ca3-be72-34144bbad02b"
            }
          ]
        },
        {
          "id": "5dc78f6d-91d5-4f17-95f9-8e8103eca477",
          "name": "get-witness-schedule",
          "request": {
            "url": "http://api.steemjs.com/get_witness_schedule",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_witness_schedule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "148e3805-d8ff-4bff-9529-995c664a991b"
            }
          ]
        },
        {
          "id": "bb836cce-0da6-4c15-9da8-9b9d4864b903",
          "name": "get-witness-by-account",
          "request": {
            "url": "http://api.steemjs.com/get_witness_by_account?accountName=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_witness_by_account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb228e2e-76f8-4b78-bf4a-86efa80843e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "f24f357b-7888-41ff-92db-4155d18a6e01",
          "name": "lookup-witness-accounts-regex-search",
          "request": {
            "url": "http://api.steemjs.com/lookup_witness_accounts?limit=%7B%7D&lowerBoundName=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "lookup_witness_accounts regex search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfc2f8aa-da36-4ddb-ad1c-cc9a0c64105c"
            }
          ]
        }
      ]
    },
    {
      "name": "Witness",
      "item": [
        {
          "id": "2fc9b048-f07f-4772-8424-710538d86fca",
          "name": "witness-update",
          "request": {
            "url": "http://api.steemjs.com/witness_update?block_signing_key=%7B%7D&fee=%7B%7D&owner=%7B%7D&props=%7B%7D&url=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "witness_update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "347bc5c1-7c9b-4bb6-9229-a34894b7783c"
            }
          ]
        }
      ]
    }
  ]
}