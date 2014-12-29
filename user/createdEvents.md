### **user/createdEvents/{uid}**

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

http://api.denzel.dev.charged.fm/user/createdEvents/1157?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "total": 1,
    "offset": 0,
    "limit": 10,
    "data": [
         {
            "id": 77,
            "event": {
                "id": 1954,
                "title": "The Grinch Who Stole Christmas",
                "time": "2014-12-26T20:00:00-05:00",
                "images": {
                    "small": "http://media.charged.fm/photos/performer/local/thumb.jpg",
                    "medium": "http://media.charged.fm/photos/performer/local/single.jpg",
                    "large": "http://media.charged.fm/photos/performer/local/single.jpg"
                },
                "url": "http://www.charged.fm/userevent/item/1954/the-grinch-who-stole-christmas",
                "performer": "",
                "venue": {
                    "name": "The Buell Theatre",
                    "address": {
                        "address_line1": "1031 13th St. ",
                        "address_line2": "",
                        "city": "Denver",
                        "state": "Colorado",
                        "country": "United States",
                        "zipcode": "80204"
                    },
                    "location": {
                        "lat": "",
                        "lng": ""
                    }
                },
                "type": "userevent",
                "isfollowing": true
            },
            "time": "2014-12-09T21:41:24-05:00"
        }
    ]
}
```
