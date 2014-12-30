### **event/details/{id}**

Deployed on branch: `dev`

#### **Description**

Get detailed event information.

#### **Method**

GET

#### **Param**

- access_token
- id: event id

Example:

http://api.dev.charged.fm/event/details/2658651?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "id": 2658651,
    "title": "Brooklyn Nets vs. New York Knicks",
    "time": "2015-02-06 19:00:00",
    "canceled": 0,
    "url": "http://www.charged.fm/new-york-knicks-tickets/brooklyn-nets-vs-new-york-knicks/02-06-2015/barclays-center/nba/2658651",
    "taxonomy": {
        "id": 10307,
        "category": "NBA",
        "parent": {
            "id": 103,
            "category": "Basketball",
            "parent": {
                "id": 1,
                "category": "Sports",
                "parent": null
            }
        }
    },
    "performers": [
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
            }
        },
        {
            "id": 307,
            "name": "Brooklyn Nets",
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
                "followers": 0,
                "broadcasts": 0
            }
        }
    ],
    "venue": {
        "id": 20182,
        "name": "Barclays Center",
        "url": "http://www.charged.fm/venue/item/20182/barclays-center",
        "address": {
            "address_line1": "Atlantic Avenue",
            "address_line2": "",
            "city": "Brooklyn",
            "state": "New York",
            "zipcode": "11217",
            "country": "United States of America"
        },
        "location": {
            "lat": 40.684193673387,
            "lng": -73.9774425
        }
    },
    "popularity": 4010,
    "counts": {
        "followers": 0,
        "broadcasts": 0
    },
    "tickets": {
        "price_lowest": 16,
        "price_highest": 7200,
        "quantity": 1337
    },
    "isfollowing": true
}
```
