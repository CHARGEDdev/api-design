### **performer/search**

Deployed on branch: `api` `dev`

#### **Description**

Search for any performer using a query string, plus any of the optional parameters below

#### **Method**

GET

#### **Param**

- q: search terms
- offset: pagination offset
- limit: pagination size limit
- cid: search for performers from a specifc category/taxonomy

Examples:
* Alt J: http://api.dev.charged.fm/performer/search?q=alt%20j
* NBA: http://api.dev.charged.fm/performer/search?cid=10307&limit=5

```javascript
{
    "total": 1,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": "43747",
            "name": "Alt-J",
            "nickname": "",
            "url": "http://www.charged.fm/alt-j-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_54bfcace60b1a.jpg",
                "medium": "http://media.charged.fm/photos/file_54bfcacea45cd.jpg",
                "large": "http://media.charged.fm/photos/file_54bfcace68ae0.jpg"
            },
            "taxonomy": {
                "id": "210",
                "category": "Indie",
                "parent": {
                    "id": "2",
                    "category": "Concert",
                    "parent": null
                }
            },
            "counts": {
                "followers": 2,
                "broadcasts": 0
            },
            "score": 8.610401
        }
    ]
}
```
