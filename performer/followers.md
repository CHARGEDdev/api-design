### **performer/followers/{performerid}**

Deployed on branch: `dev`

#### **Description**

Get a list of users following specific performer.

#### **Method**

Get

#### **Param**

- performer id
- access_token
- offset: default 0
- limit: default 10

Example:

http://api.dev.charged.fm/performer/followers/389?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "total": 1,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": 3,
            "user": {
                "id": 1157,
                "username": "ZZZ",
                "email": "denzel@charged.fm",
                "fullname": "first last",
                "gender": "Male",
                "birthday": "0000-00-00",
                "biography": "",
                "dashboard": "http://www.charged.fm/office/dashboard",
                "avatar": "http://media.charged.fm/media/file_54cad7dc300a0.jpg",
                "thumb": "http://media.charged.fm/media/file_54cad7dc30107.jpg",
                "counts": {
                    "following_users": 237,
                    "followers": 249,
                    "following_peformers": 8,
                    "following_events": 9,
                    "broadcasts": 0,
                    "userevents": 0
                },
                "isfollowing": false
            },
            "time": "2015-02-02T17:17:16-05:00"
        }
    ]
}
```
