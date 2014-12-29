### **user/attendingEvents/{uid}**

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

http://api.denzel.dev.charged.fm/user/attendingEvents/1157?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "total": 1,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": 2,
            "event": {
                "id": 2531872,
                "title": "New York Giants vs. Philadelphia Eagles",
                "time": "2014-12-28 13:00:00",
                "canceled": 0,
                "url": "http://www.charged.fm/new-york-giants-tickets/new-york-giants-vs-philadelphia-eagles/12-28-2014/metlife-stadium-formerly-new-meadowlands-stadium/nfl/2531872",
                "taxonomy": {
                    "id": 10804,
                    "category": "NFL",
                    "parent": {
                        "id": 108,
                        "category": "Football",
                        "parent": {
                            "id": 1,
                            "category": "Sports",
                            "parent": null
                        }
                    }
                },
                "performers": [
                    {
                        "id": 50202,
                        "name": "New York Giants",
                        "url": "http://www.charged.fm/new-york-giants-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_5453a5e4ade0d.jpg",
                            "medium": "http://media.charged.fm/photos/file_5453a5e518366.jpg",
                            "large": "http://media.charged.fm/photos/file_5453a5e4bc99c.jpg"
                        },
                        "taxonomy": {
                            "id": "10804",
                            "category": "NFL",
                            "parent": {
                                "id": "108",
                                "category": "Football",
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
                        "id": 350,
                        "name": "Philadelphia Eagles",
                        "url": "http://www.charged.fm/philadelphia-eagles-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_5417014e11bd1.jpg",
                            "medium": "http://media.charged.fm/photos/file_5417014ea6e29.jpg",
                            "large": "http://media.charged.fm/photos/file_5417014e3c980.jpg"
                        },
                        "taxonomy": {
                            "id": "10804",
                            "category": "NFL",
                            "parent": {
                                "id": "108",
                                "category": "Football",
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
                    "id": 23199,
                    "name": "MetLife Stadium (Formerly New Meadowlands Stadium)",
                    "url": "http://www.charged.fm/venue/item/23199/metlife-stadium-formerly-new-meadowlands-stadium",
                    "address": {
                        "address_line1": "One MetLife Stadium Dr.",
                        "address_line2": "",
                        "city": "East Rutherford",
                        "state": "New Jersey",
                        "zipcode": "07073",
                        "country": "United States of America"
                    },
                    "location": {
                        "lat": 40.8141282,
                        "lng": -74.0737144
                    }
                },
                "popularity": 0,
                "counts": {
                    "followers": 0,
                    "broadcasts": 0
                },
                "tickets": {
                    "price_lowest": 0,
                    "price_highest": 0,
                    "quantity": 0
                },
                "type": "event",
                "isfollowing": true
            },
            "time": "1969-12-31T19:00:00-05:00"
        }
    ]
}
```
