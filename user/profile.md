### **user/profile/{uid}**

Deployed on branch: `dev`

#### **Description**

#### **Method**

Get

#### **Param**

- uid
- access_token

Example:

http://api.dev.charged.fm/user/profile/4?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "id": 1,
    "username": "pLot",
    "email": "devleads@plotmulti.com",
    "fullname": "pLot Developers",
    "gender": "Male",
    "birthday": "0000-00-00",
    "dashboard": "http://www.charged.fm/office/dashboard",
    "avatar": "http://media.charged.fm/media/file_4e00bba66da37.jpg",
    "thumb": "http://media.charged.fm/media/file_4e00bba744d3d.jpg",
    "counts": {
        "following_users": 0,
        "followers": 0,
        "following_peformers": 0,
        "following_events": 0,
        "broadcasts": 0,
        "userevents": 0
    },
    "isfollowing": false
}
```
