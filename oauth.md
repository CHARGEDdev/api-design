### **oauth**

Deployed on branch: `api` `dev`

#### **Description**

Oauth sign in endpoint. Two types of sign in methods are supported:

1. Regular: sign in with CHARGED.fm `email` and `password`
2. Social: sign in with `Facebook` 

#### **Method**

GET

#### **Param**

- `client_id`: app id
- `redirect_uri`: app redirect uri
- `scope`: permission scopes
- `response_type`: always be `code`
- `type`: optional, type of social network sign in. `facebook` is supported 
  - `facebook_access_token`: required if `type=facebook`

Response:

```
http://charged/oauth?code=2c0adaae26873757f170471c3366fb9a&state=
```

