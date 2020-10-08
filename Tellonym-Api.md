## INSTAGRAM : @qq_iq 😊💜
# Tellonym-Api :

## Get Req :
  Token Header Name : Authorization
  ### Account private info :
      https://api.tellonym.me/accounts/myself?limit=13

  ### Account Friends :
      https://api.tellonym.me/suggestions/friends?limit=13

  ### Account Tells : 
      https://api.tellonym.me/tells?limit=13

  ### Account notifications :
      https://api.tellonym.me/notifications?filterBlacklist%5B0%5D=3&limit=13

## POST Req:
  ### Create Tellonym Token :
    URL : https://api.tellonym.me/tokens/create
    Headers : Accept = application/json & user-agent
    JSON :
    {
      "deviceName": "User Agent Here",
      "deviceType": "web",
      "lang": "en",
      "captcha": "",
      "email": "",
      "password": "",
      "limit": 13
    }

    And The Response is a Json :
    accessToken = is the token you created
    userId = Account UserId
    type = Login 

  ### Logout  :
      URL : https://api.tellonym.me/tokens/destroy

  ### Change User Info & Username : 
      URL : https://api.tellonym.me/accounts/settings
      Headers : Authorization = "Token"
      json : 
      {
        "instagram": "",
        "snapchat": "",
        "twitter": "",
        "username": "",
        "limit": 13
      }

