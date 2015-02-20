### **import/friends**

Deployed on branch: `api` `dev`

#### **Description**

Friends import script from different social networks.

An array of suggest friends will be returned to user to decide whether to follow or now.

It's a one time running script, it wouldnt store data on server.

`isfollowing` field is returned to indicate whether user has already been followed.

#### **Method**

GET

#### **Param**

- access_token
- from: source of connection. available sources are `facebook`
- facebook_access_token: mandatory if `from` is `facebook`

Example:

Request:
```sh
curl 'http://api.dev.charged.fm/import/friends?access_token=charged_access_token&from=facebook&facebook_access_token=facebook_token'
```

Response:
```javascript
[
    {
        "id": 243,
        "username": "",
        "email": "h@gmail.com",
        "fullname": "Henrik",
        "gender": "Male",
        "birthday": "1985-04-09",
        "biography": "",
        "dashboard": "http://www.charged.fm/dashboard",
        "avatar": "http://media.charged.fm/media/file_50a2c2a92cc39.jpg",
        "thumb": "http://media.charged.fm/media/file_50a2c2a92d3f9.jpg",
        "counts": {
            "following_users": "0",
            "followers": "0",
            "following_peformers": "1",
            "following_events": "0",
            "broadcasts": "0",
            "userevents": "0"
        },
        "isfollowing": false
    },
    {
        "id": 994,
        "username": "",
        "email": "andrew@gmail.com",
        "fullname": "Andrew",
        "gender": "Male",
        "birthday": "1988-08-28",
        "biography": "",
        "dashboard": "http://www.charged.fm/dashboard",
        "avatar": "http://media.charged.fm/media/file_50a2cef315f52.jpg",
        "thumb": "http://media.charged.fm/media/file_50a2cef31671c.jpg",
        "counts": {
            "following_users": 0,
            "followers": 0,
            "following_peformers": 0,
            "following_events": 0,
            "broadcasts": 0,
            "userevents": 0
        },
        "isfollowing": false
    },
    .
    .
    .
    {
        "id": 118539,
        "username": "",
        "email": "testshen@hotmail.com",
        "fullname": "test  Shen ",
        "gender": "Male",
        "birthday": "1989-09-05",
        "biography": "",
        "dashboard": "http://www.charged.fm/dashboard",
        "avatar": "http://media.charged.fm/media/file_5446c5deebfef.jpg",
        "thumb": "http://media.charged.fm/media/file_5446c5deec0b0.jpg",
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
]
```



