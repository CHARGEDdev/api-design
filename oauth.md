### **oauth**

Deployed on branch: `api` `dev`

#### **Description**

Oauth sign in endpoind. Two type of sign in method supported.

1. normal `email` `password` sign in
2. sign in with facebook

#### **Method**

GET

#### **Param**

- client_id: app id
- redirect_uri: app redirect uri
- scope: permission scopes
- response_type: always be `code`
- type: optional, type of social network sign in. `facebook` is supported 
- facebook_access_token: mandatory if `type` is `facebook`

Response:

```
http://charged/oauth?code=2c0adaae26873757f170471c3366fb9a&state=
```

