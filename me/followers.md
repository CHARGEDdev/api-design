### **me/followers**

Deployed on branch: `api` `dev`

#### **Description**

Returns all users that the logged-in user is followed by

#### **Method**

GET

#### **Param**

- total
- offset
- limit
- data

Example:
http://api.charged.fm/me/followers

```javascript

{
    "total": 1,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": 214,
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
                    "following_peformers": "0",
                    "following_events": "0",
                    "broadcasts": "0"
                },
                "isfollowing": true
            },
            "time": "2014-09-05T19:13:39-04:00"
        }
    ]
}
```
