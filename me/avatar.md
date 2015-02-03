### **me/avatar**

Deployed on branch: `dev`

#### **Description**

Update user's profile image, return the updated user profile if success.

#### **Method**

POST

#### **Param**

- access_token
- avatar: image file, either `image/jpeg`, `image/png`

Example:

Response:

```javascript
{
    "id": 1157,
    "username": "Z",
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
    }
}
```
