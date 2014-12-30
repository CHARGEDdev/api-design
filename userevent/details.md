### **userevent/details/{id}**

Deployed on branch: `dev`

#### **Description**

Get detailed userevent information.

#### **Method**

GET

#### **Param**

- access_token
- id: userevent id

Example:

http://api.dev.charged.fm/userevent/details/1954?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
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
    "counts": {
        "followers": 0,
        "broadcasts": 0
    },
    "isfollowing": true
}
```
