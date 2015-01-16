### **me/broadcasts**

Deployed on branch: `api` `dev`

#### **Description**

Returns profile for the logged in user

#### **Method**

GET

#### **Param**

    "id": 67597,
    "username": "",
    "email": "support8@charged.fm",
    "fullname": "Marc Sabin",
    "gender": "",
    "birthday": "0000-00-00",
    "dashboard": "http://www.charged.fm/office/dashboard",
    "avatar": "http://www.charged.fm/images/user/profile-single.jpg",
    "thumb": "http://www.charged.fm/images/user/profile-thumb.jpg",
    "counts": {
        "following_users": 0,
        "followers": 0,
        "following_peformers": 0,
        "following_events": 0,
        "broadcasts

- id
- username
- 
- 
- 
- 
- access_token
- offset: default 0
- limit: default 10


Example:
http://api.charged.fm/me/profile

```javascript

{
    "id": 67597,
    "username": "",
    "email": "support8@charged.fm",
    "fullname": "Marc Sabin",
    "gender": "",
    "birthday": "0000-00-00",
    "dashboard": "http://www.charged.fm/office/dashboard",
    "avatar": "http://www.charged.fm/images/user/profile-single.jpg",
    "thumb": "http://www.charged.fm/images/user/profile-thumb.jpg",
    "counts": {
        "following_users": 0,
        "followers": 0,
        "following_peformers": 0,
        "following_events": 0,
        "broadcasts": 0
    }
}
```
