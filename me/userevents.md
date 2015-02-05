### **me/userevents**

Deployed on branch: `api` `dev`

#### **Description**

Returns userevents for the logged in user

#### **Method**

GET

#### **Param**

- total
- offset
- limit
- min_year
- max_year

Example:
http://api.charged.fm/me/userevents

```javascript
{
    "total": 2,
    "offset": 0,
    "limit": 1000,
    "min_year": 0,
    "max_year": 0,
    "data": [
        {
            "id": 1875,
            "title": "Totally Awesome Event",
            "time": "2014-10-14T17:30:00-04:00",
            "images": {
                "small": "http://media.charged.fm/media/file_543700223a866.jpg",
                "medium": "http://media.charged.fm/media/file_5437002378c34.jpg",
                "large": "http://media.charged.fm/media/file_54370022902bf.jpg"
            },
            "url": "http://www.charged.fm/userevent/item/1875/totally-awesome-event",
            "performer": "Me",
            "venue": {
                "name": "Madison Square Garden",
                "address": {
                    "address_line1": "4 Pennsylvania Plaza",
                    "address_line2": "",
                    "city": "New York",
                    "state": "New York",
                    "country": "United States",
                    "zipcode": "10001"
                },
                "location": {
                    "lat": "",
                    "lng": ""
                }
            }
        },
        {
            "id": 1878,
            "title": "Testish",
            "time": "2015-02-28T19:30:00-05:00",
            "images": {
                "small": "http://media.charged.fm/photos/performer/local/thumb.jpg",
                "medium": "http://media.charged.fm/photos/performer/local/single.jpg",
                "large": "http://media.charged.fm/photos/performer/local/single.jpg"
            },
            "url": "http://www.charged.fm/userevent/item/1878/testish",
            "performer": "Me",
            "venue": {
                "name": "Derp",
                "address": {
                    "address_line1": "111 W State St",
                    "address_line2": "",
                    "city": "West Lafayette",
                    "state": "Indiana",
                    "country": "United States",
                    "zipcode": "46526"
                },
                "location": {
                    "lat": "",
                    "lng": ""
                }
            }
        }
    ]
}
```
