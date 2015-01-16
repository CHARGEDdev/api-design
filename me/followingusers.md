### **me/followingusers**

Deployed on branch: `api` `dev`

#### **Description**

Returns all users that the logged-in user is following

#### **Method**

GET

#### **Param**

- total
- offset
- limit
- data

Example:
http://api.charged.fm/me/followingusers

```javascript

{
    "total": 1,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": 464,
            "user": {
                "id": 1157,
                "username": "Z",
                "email": "",
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
            "time": "2014-09-05T19:17:49-04:00"
        }
    ]
}
```
