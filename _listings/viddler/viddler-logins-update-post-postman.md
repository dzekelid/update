{
  "info": {
    "name": "Viddler  API Logins Update",
    "_postman_id": "6b1e249b-77b7-4709-92b9-ca27ec4363e5",
    "description": "Updates a current login.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "fbe4abde-df6f-40d1-8366-559c17ea4710",
          "name": "api-echo",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.api.echo?message=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method is used for testing purposes only. Simply call this method to make sure the API is responding fine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04237d83-e91d-41e0-b498-90155ba3c48a"
            }
          ]
        },
        {
          "id": "f5b7f898-1c9c-4520-a11b-abc88a37ce40",
          "name": "encoding-cancel",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.encoding.cancel?file_id=%7B%7D&sessionid=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Cancel encoding a specific video file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "960c86d6-2f92-4bbf-be9b-bc104391b7a5"
            }
          ]
        },
        {
          "id": "52d4e71f-41d6-43f8-a425-66793c3eeb80",
          "name": "encoding-getsettings",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.encoding.getSettings?sessionid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current encoding options for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "726373e0-ce10-480c-8d72-a2cb3ab150b9"
            }
          ]
        },
        {
          "id": "b02797df-2ab0-441d-a48f-ea538f1aebf1",
          "name": "encoding-getstatus2",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.encoding.getStatus2?sessionid=%7B%7D&video_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method is the same as viddler.encoding.getStatus except that it groups files better for users to easily find what they are looking for. We could not easily update the previous method without causing complications with external applications."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bc48f7b-e21e-408d-b4d4-d28df5b64867"
            }
          ]
        },
        {
          "id": "ae3179b0-1980-433c-b2bf-4ab8c26f690f",
          "name": "logins-add",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.logins.add?analytics_permissions=%7B%7D&api_access_permissions=%7B%7D&api_settings_permissions=%7B%7D&billing_settings_permissions=%7B%7D&branding_settings_permissions=%7B%7D&email=%7B%7D&encoding_settings_permissions=%7B%7D&interaction_settings_permissions=%7B%7D&invoices_permissions=%7B%7D&itunes_settings_permissions=%7B%7D&login=%7B%7D&logins_permissions=%7B%7D&name=%7B%7D&password=%7B%7D&player_settings_permissions=%7B%7D&playlists_permissions=%7B%7D&playlist_ids=%7B%7D&privacy_settings_permissions=%7B%7D&profile_permissions=%7B%7D&recorder_permissions=%7B%7D&sessionid=%7B%7D&subaccounts_permissions=%7B%7D&support_permissions=%7B%7D&videos_permissions=%7B%7D&vidgets_permissions=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new login to user account when the main account has multi-user sign-on enabled. You must have this feature enabled for your account. Please call us at 1-888-444-1119 to enable for you account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e728277-3736-424b-abef-37a45d809b3e"
            }
          ]
        },
        {
          "id": "95d771fe-a92b-4b07-a69c-2988a5755e3b",
          "name": "logins-get",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.logins.get?login=%7B%7D&sessionid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the current permissions for a specific user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9f5415e-71c5-4e92-beaa-06067b2a74ea"
            }
          ]
        },
        {
          "id": "5aec5ca4-1e4b-46fc-a951-2ac6aa7df404",
          "name": "logins-update",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.logins.update?analytics_permissions=%7B%7D&api_access_permissions=%7B%7D&api_settings_permissions=%7B%7D&billing_settings_permissions=%7B%7D&branding_settings_permissions=%7B%7D&email=%7B%7D&encoding_settings_permissions=%7B%7D&interaction_settings_permissions=%7B%7D&invoices_permissions=%7B%7D&itunes_settings_permissions=%7B%7D&login=%7B%7D&logins_permissions=%7B%7D&name=%7B%7D&password=%7B%7D&player_settings_permissions=%7B%7D&playlists_permissions=%7B%7D&playlist_ids=%7B%7D&privacy_settings_permissions=%7B%7D&profile_permissions=%7B%7D&recorder_permissions=%7B%7D&sessionid=%7B%7D&subaccounts_permissions=%7B%7D&support_permissions=%7B%7D&videos_permissions=%7B%7D&vidgets_permissions=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a current login."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a73a0256-e729-421d-92c7-eabfe97a0542"
            }
          ]
        }
      ]
    }
  ]
}