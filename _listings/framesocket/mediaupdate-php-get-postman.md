{
  "info": {
    "name": "Framesocket Update Media",
    "_postman_id": "fc095921-62b3-4576-a650-8ee19423f4dd",
    "description": "Update Media",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Media",
      "item": [
        {
          "id": "4768ac9e-fd96-4913-a34a-65fb88cb588b",
          "name": "getMediaActivate.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/activate.php?customid=%7B%7D&hash=%7B%7D&key=%7B%7D&secret=%7B%7D&sig=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activate Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bb9f463-7525-4045-ad4b-9300986a6468"
            }
          ]
        },
        {
          "id": "32c0e05b-ba94-4743-85c1-e7413a5837ce",
          "name": "getMediaDeactivate.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/deactivate.php?customid=%7B%7D&hash=%7B%7D&key=%7B%7D&secret=%7B%7D&sig=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deactive Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c471e91f-bdb9-4dc6-a1d7-3cf4afe749d0"
            }
          ]
        },
        {
          "id": "fb8cf493-834d-408c-941e-81408acc0aae",
          "name": "getMediaImages.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/images.php?customid=%7B%7D&hash=%7B%7D&key=%7B%7D&secret=%7B%7D&sig=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query Images"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6d3d6e0-5e77-49e7-9af6-8f867dceeddf"
            }
          ]
        },
        {
          "id": "82df264e-bc39-4a71-bf9c-3df79939a94c",
          "name": "getMediaQuery.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/query.php?andkeywords=%7B%7D&andtitlewords=%7B%7D&customid=%7B%7D&hash=%7B%7D&key=%7B%7D&limit=%7B%7D&orkeywords=%7B%7D&ortitlewords=%7B%7D&secret=%7B%7D&sig=%7B%7D&sort=%7B%7D&status=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a9aef10-3a25-4168-95ec-41bbe8eec432"
            }
          ]
        },
        {
          "id": "b6aab5d3-610e-4613-b53f-84ea6178462b",
          "name": "getMediaUpdate.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/update.php?customid=%7B%7D&description=%7B%7D&hash=%7B%7D&imagehash=%7B%7D&key=%7B%7D&keywords=%7B%7D&secret=%7B%7D&sig=%7B%7D&title=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Update Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "975d3a43-4c84-4601-aea8-99c32960d64e"
            }
          ]
        }
      ]
    }
  ]
}