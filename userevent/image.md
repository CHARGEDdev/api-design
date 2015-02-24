### **userevent/image**

Deployed on branch: `dev`

#### **Description**

Set an image for the userevent

#### **Method**

POST

#### **Param**

- `access_token`: your access token, (required)
- `mediaID`: a media id from your [media library `media/images`](https://github.com/denzeus/api-design/blob/master/media/images.md). Upload an image to your media library using the [`media/image`](https://github.com/denzeus/api-design/blob/master/media/image.md) endpoint. (required)
- `eventID`: the userevent id (required)

Example:

```javascript
{
    "status": "success",
    "data": {
        "id": "2118",
        "userID": "3",
        "title": "SXBK",
        "description": "South By South Brooklyn",
        "startDate": "2015-03-01 19:15:00",
        "endDate": "0000-00-00 00:00:00",
        "venue": {
            "name": "CHARGED.fm",
            "address": {
                "address_line1": "",
                "address_line2": "",
                "city": "Brooklyn",
                "state": "NY",
                "zipcode": "10017",
                "country": "United States"
            },
            "location": {
                "lat": 40.704578,
                "lng": -73.986794
            }
        },
        "tags": "",
        "category": "1",
        "subcategory": "0",
        "public": 1,
        "url": "http://www.charged.fm/userevent/item/2118",
        "created": "0000-00-00 00:00:00",
        "published": "1",
        "datePublished": "2015-02-23 10:40:08",
        "updated": "2015-02-24 14:56:50",
        "tickets": {
            "price_highest": "10.25",
            "price_lowest": "5.00",
            "quantity": "2",
            "tickets": [
                {
                    "id": "3964",
                    "name": "Early Bird",
                    "description": "Hey",
                    "type": "regular",
                    "price": "10.25",
                    "capacity": "100",
                    "remaining": "96",
                    "sellStartDate": "2015-02-20 00:00:00",
                    "sellEndDate": "0000-00-00 00:00:00",
                    "minPerOrder": "1",
                    "maxPerOrder": "4",
                    "feeOption": "1"
                },
                {
                    "id": "3970",
                    "name": "GA",
                    "description": "Test update ticket",
                    "type": "regular",
                    "price": "5.00",
                    "capacity": "0",
                    "remaining": "0",
                    "sellStartDate": "0000-00-00 00:00:00",
                    "sellEndDate": "0000-00-00 00:00:00",
                    "minPerOrder": "0",
                    "maxPerOrder": "0",
                    "feeOption": "1"
                }
            ]
        },
        "images": {
            "square_small": {
                "url": "http://media.charged.fm/photos/usergen/events/2118square_small1424815063.jpg",
                "width": "160",
                "height": "160"
            },
            "square_standard": {
                "url": "http://media.charged.fm/photos/usergen/events/2118square_standard1424815062.jpg",
                "width": "320",
                "height": "320"
            },
            "square_large": {
                "url": "http://media.charged.fm/photos/usergen/events/2118square_large1424815062.jpg",
                "width": "640",
                "height": "640"
            },
            "banner": {
                "url": "http://media.charged.fm/photos/usergen/events/2118banner1424815061.jpg",
                "width": "1024",
                "height": "576"
            }
        }
    },
    "code": 200
}
```
