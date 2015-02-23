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

Example Request:

Normal user login: 
```sh
curl http://api.charged.fm/oauth?client_id=app_id&redirect_uri=http://charged/oauth&scope=god&response_type=code
```

Facebook user login: 
```sh
curl http://api.charged.fm/oauth?client_id=app_id&redirect_uri=http://charged/oauth&scope=god&response_type=code
&type=facebook&facebook_access_token=your_fb_token
```

Response:

```
http://charged/oauth?code=2c0adaae26873757f170471c3366fb9a&state=
```

