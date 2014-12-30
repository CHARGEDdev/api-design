### **user/followingPerformers/{uid}**

Deployed on branch: `dev`

#### **Description**

#### **Method**

GET

#### **Param**

- uid
- access_token
- offset: default 0
- limit: default 10

Example:

http://api.dev.charged.fm/user/followingPerformers/1157?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "total": 2,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": 3,
            "performer": {
                "id": 389,
                "name": "San Diego Padres",
                "url": "http://www.charged.fm/san-diego-padres-tickets",
                "images": {
                    "small": "http://media.charged.fm/photos/file_54206433d4dc0.jpg",
                    "medium": "http://media.charged.fm/photos/file_542064340ff91.jpg",
                    "large": "http://media.charged.fm/photos/file_54206433dcbf0.jpg"
                },
                "taxonomy": {
                    "id": "10205",
                    "category": "MLB",
                    "parent": {
                        "id": "102",
                        "category": "Baseball",
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
                "isfollowing": true
            },
            "time": "2014-12-02T14:25:18-05:00"
        },
        {
            "id": 1,
            "performer": {
                "id": 315,
                "name": "New York Yankees",
                "url": "http://www.charged.fm/new-york-yankees-tickets",
                "images": {
                    "small": "http://media.charged.fm/photos/file_54203c440a645.jpg",
                    "medium": "http://media.charged.fm/photos/file_54203c446026f.jpg",
                    "large": "http://media.charged.fm/photos/file_54203c441992a.jpg"
                },
                "taxonomy": {
                    "id": "10205",
                    "category": "MLB",
                    "parent": {
                        "id": "102",
                        "category": "Baseball",
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
                "isfollowing": true
            },
            "time": "1969-12-31T19:00:00-05:00"
        }
    ]
}
```
