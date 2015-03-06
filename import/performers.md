### **import/performers**

Deployed on branch: `api` `dev`

#### **Description**

Performer import script. Only matched performers will be returned. It's a one time running script, it wouldnt store data on server. `isfollowing` field is returned to indicate whether performer has already been followed.

#### **Method**

POST

#### **Param**

- access_token
- autofollow: if this param is presented in url, user will auto follow suggested performers.
- data: json encoded array of performers

Example:

Request:
```sh
curl 'http://api.charged.fm/import/performers?access_token=token' \
-F 'data=["nets","knicks","taylor"]'
```
Auto follow performers
```sh
curl 'http://api.charged.fm/import/performers?access_token=token&autofollow' \
-F 'data=["nets","knicks","taylor"]'
```


Response:
```javascript
[
    {
        "id": "307",
        "name": "Brooklyn Nets",
        "nickname": "Nets",
        "url": "http://www.charged.fm/brooklyn-nets-tickets",
        "images": {
            "small": "http://media.charged.fm/photos/file_540f5e157b440.jpg",
            "medium": "http://media.charged.fm/photos/file_540f5e1666cce.jpg",
            "large": "http://media.charged.fm/photos/file_540f5e15a6c6b.jpg"
        },
        "taxonomy": {
            "id": "10307",
            "category": "NBA",
            "parent": {
                "id": "103",
                "category": "Basketball",
                "parent": {
                    "id": "1",
                    "category": "Sports",
                    "parent": null
                }
            }
        },
        "counts": {
            "followers": 2,
            "broadcasts": 0
        },
        "score": 8.142126,
        "isfollowing": false
    },
    {
        "id": "312",
        "name": "New York Knicks",
        "nickname": "Knicks",
        "url": "http://www.charged.fm/new-york-knicks-tickets",
        "images": {
            "small": "http://media.charged.fm/photos/file_5407b6c15d1ba.jpg",
            "medium": "http://media.charged.fm/photos/file_5407b6c33739c.jpg",
            "large": "http://media.charged.fm/photos/file_5407b6c1eb155.jpg"
        },
        "taxonomy": {
            "id": "10307",
            "category": "NBA",
            "parent": {
                "id": "103",
                "category": "Basketball",
                "parent": {
                    "id": "1",
                    "category": "Sports",
                    "parent": null
                }
            }
        },
        "counts": {
            "followers": 0,
            "broadcasts": 0
        },
        "score": 7.855419,
        "isfollowing": false
    }
]
```

#### **Method**

GET

#### **Param**

- access_token
- autofollow: if this param is presented in url, user will auto follow suggested performers.
- from: source of connection. available sources are facebook, spotify
- facebook_access_token: mandatory if from is facebook
- spotify_access_token: mandatory if from is spotify

Example:

Request:
```sh
curl 'http://api.dev.charged.fm/import/performers?access_token=charged_access_token&from=facebook&facebook_access_token=facebook_token'
```
Auto follow: 
```sh
curl 'http://api.dev.charged.fm/import/performers?access_token=charged_access_token&from=facebook&facebook_access_token=facebook_token&autofollow'
```

Response:
```javascript
[
    {
        "id": "62",
        "name": "Bob Dylan",
        "nickname": "",
        "url": "http://www.charged.fm/bob-dylan-tickets",
        "images": {
            "small": "http://media.charged.fm/photos/file_542343567ce6f.jpg",
            "medium": "http://media.charged.fm/photos/file_54234356e33e1.jpg",
            "large": "http://media.charged.fm/photos/file_5423435694267.jpg"
        },
        "taxonomy": {
            "id": "201",
            "category": "Classic Rock",
            "parent": {
                "id": "2",
                "category": "Concert",
                "parent": null
            }
        },
        "counts": {
            "followers": 0,
            "broadcasts": 0
        },
        "score": 7.233924,
        "isfollowing": false
    }
]
```



