### **event/search**

Deployed on branch: `api` `dev`

#### **Description**

Search for any event using a query string, plus optional parameters below

#### **Method**

GET

#### **Param**

- q: search terms
- offset: pagination offset
- limit: pagination size limit
- latlng: comma sperated latlng, example: 40.723301,-74.0029883
- radius: default to 5 miles.
- latlng.ne: bounds search northeast, example: 40.7283442,-73.9958967
- latlng.sw: bounds search southwest, example: 40.7189454,-74.0054619
- pid: search for event of a performer
- cid: search for event of a category
- verbose: append &verbose to enable verbose output, no value needed.

Examples:
* http://api.dev.charged.fm/event/search?limit=100&offset=100&q=new%20york%20yankees
* http://api.dev.charged.fm/event/search?latlng=40.7286587,-73.9925526&radius=1&limit=100&offset=100
* http://api.dev.charged.fm/event/search?pid=321
* http://api.dev.charged.fm/event/search?cid=306&verbose
* http://api.dev.charged.fm/event/search?cid=1&latlng=40.7286587,-73.9925526

```javascript
{
    "total": 30,
    "offset": 0,
    "limit": 1,
    "data": [
        {
            "id": "2658572",
            "title": "Brooklyn Nets vs. Portland Trail Blazers",
            "nickname": "Nets vs. Trail Blazers",
            "time": "2015-04-06 19:00:00",
            "images": {
                "small": "http://media.charged.fm/photos/file_54087fd2da6b6.jpg",
                "medium": "http://media.charged.fm/photos/file_54087fd6b2e98.jpg",
                "large": "http://media.charged.fm/photos/file_54087fd426ece.jpg"
            },
            "performers": [
                {
                    "id": 50215,
                    "name": "Portland Trail Blazers",
                    "images": {
                        "small": "http://media.charged.fm/photos/file_54087fd2da6b6.jpg",
                        "medium": "http://media.charged.fm/photos/file_54087fd6b2e98.jpg",
                        "large": "http://media.charged.fm/photos/file_54087fd426ece.jpg"
                    }
                },
                {
                    "id": 307,
                    "name": "Brooklyn Nets",
                    "images": {
                        "small": "http://media.charged.fm/photos/file_540f5e157b440.jpg",
                        "medium": "http://media.charged.fm/photos/file_540f5e1666cce.jpg",
                        "large": "http://media.charged.fm/photos/file_540f5e15a6c6b.jpg"
                    }
                }
            ],
            "venue": {
                "id": 20182,
                "name": "Barclays Center",
                "location": {
                    "lat": "40.684193673387",
                    "lng": "-73.9774425"
                }
            },
            "popularity": 6319,
            "counts": {
                "followers": 0,
                "broadcasts": 0
            },
            "tickets": {
                "price_lowest": 16,
                "price_highest": 414,
                "quantity": 218
            }
        }
    ]
}
```
