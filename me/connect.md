### **me/connect**

Deployed on branch: `api` | `dev`

#### **Description**

connect CHRAGED's account to other SNS like facebook, twitter, etc.

return updated user's profile if connected successfully.

#### **Method**

POST

#### **Param**

- `access_token`
- `from`: source of connection. available sources are `facebook`
- `facebook_access_token`: mandatory if `from` is facebook


#### **Example**

request

```sh
curl 'http://api.charged.fm/me/connect?access_token=token' \
-F 'from=facebook' \
-F 'facebook_access_token=token'
```

response
```javascript
{
    "id": 172393,
    "username": "zerongj",
    "email": "denzeljiang@gmail.com",
    "fullname": "Zerong Jiang",
    "gender": "Male",
    "birthday": "0000-00-00",
    "biography": "",
    "dashboard": "http://www.charged.fm/dashboard",
    "avatar": "http://media.charged.fm/media/file_54dce273e5e99.jpg",
    "thumb": "http://media.charged.fm/media/file_54dce273e604a.jpg",
    "counts": {
        "following_users": 0,
        "followers": 0,
        "following_peformers": 0,
        "following_events": 0,
        "broadcasts": 0,
        "userevents": 0
    },
    "connections": [
        {
            "type": "facebook",
            "identity": "denzeljiang@gmail.com"
        }
    ]
}
```
