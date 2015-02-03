### **me/profile**

Deployed on branch: `api` `dev`

#### **Description**

Returns profile for the logged in user

#### **Method**

GET

#### **Param**

- id
- username
- email
- fullname
- gender
- birthday
- dashboard
- avatar
- thumb
- counts

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
        "broadcasts": 0,
        "userevents": 0
    }
}
```

================================================================

### **me/profile**

Deployed on branch: `dev`

#### **Description**

Update user profile, and return updated user profile if success.

#### **Method**

PUT

#### **Param**

- `access_token`
- `firstname`: optional
- `lastname`: mandatory if `firstname` is present
- `email`: optional
- `gender`: optional, 'Male' or 'Female'
- `birthday`: optional, format should be 1900-01-01
- `biography`: optional, any string
- `password_old`: optional, old password
- `password`: mandatory if `password_old` is present, 5 character at least
- `password_repeat`: mandatory if `password_old` is present, 5 character at least

Example:

Request:

```sh
curl 'http://api.dev.charged.fm/me/profile?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242'
-X PUT
--data 'firstname=first&lastname=last&gender=Male'
```

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


