### **user/followers/{uid}**

Deployed on branch: `dev`

#### **Description**

#### **Method**

Get

#### **Param**

- uid
- access_token
- offset: default 0
- limit: default 10

Example:

http://api.denzel.dev.charged.fm/user/followers/5?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "total": 1,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": 2,
            "user": {
                "id": 1157,
                "username": "Z",
                "email": "denzel@charged.fm",
                "fullname": "Denzel Jiang",
                "gender": "Male",
                "birthday": "0000-00-00",
                "dashboard": "http://www.charged.fm/office/dashboard",
                "avatar": "http://media.charged.fm/media/file_501fde6e4e7c2.jpg",
                "thumb": "http://media.charged.fm/media/file_501fde6e84eda.jpg",
                "counts": {
                    "following_users": "1",
                    "followers": "0",
                    "following_peformers": "1",
                    "following_events": "0",
                    "broadcasts": "0"
                },
                "isfollowing": false
            },
            "time": "2014-09-05T19:10:07-04:00"
        }
    ]
}
```
