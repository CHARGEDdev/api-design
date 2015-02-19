### **import/performers**

Deployed on branch: `api` `dev`

#### **Description**

Performer import script. Only matched performers will be returned. It's a one time running script, it wouldnt store data on server. `isfollowing` field is returned to indicate whether performer has already been followed.

#### **Method**

POST

#### **Param**

- access_token
- data: json encoded array of performers

Example:

Request:
```sh
curl 'http://api.charged.fm/performer/import?access_token=token' \
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
