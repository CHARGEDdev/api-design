### **performer/profile/{pid}**

Deployed on branch: `dev`

#### **Description**

#### **Method**

Get

#### **Param**

- pid
- access_token

Example:

http://api.denzel.dev.charged.fm/performer/profile/312?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "id": 312,
    "name": "New York Knicks",
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
    "isfollowing": false
}
```
