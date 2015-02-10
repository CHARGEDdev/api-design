### **userevent/image**

Deployed on branch: `evan`

#### **Description**

Set an image for the userevent

#### **Method**

POST

#### **Param**

- access_token
- mediaID (Upload image using the [media/image](https://github.com/denzeus/api-design/blob/master/media/image.md) endpoint and pass in the `mediaID` you get back)
- eventID

Example:

```javascript
{
    "status": "success",
    "data": {
        "id": "459",
        "userID": "3",
        "title": "Thirsty Thursdays",
        "description": "...",
        "image": "http://media.charged.fm/photos/usergen/events/standard_1423598641_9zf5UyEF.png",
        "startDate": "2012-08-09 00:00:00",
        "endDate": "2012-08-09 00:00:00",
        "venue": {
            "name": "DUM-Beer-O-Central",
            "address": {
                "address_line1": "10 Jay St",
                "address_line2": "",
                "city": "Brooklyn",
                "state": "New York",
                "zipcode": "11201",
                "country": "United States"
            },
            "location": {
                "lat": 0,
                "lng": 0
            }
        },
        "tags": "-",
        "category": "0",
        "subcategory": "0",
        "public": "no",
        "url": "http://www.charged.fm/userevent/item/459",
        "created": "0000-00-00 00:00:00",
        "published": "0000-00-00 00:00:00",
        "updated": "2015-02-10 15:48:55",
        "tickets": [
            {
                "id": "1077",
                "name": "Easy Goin'",
                "description": "RSVP and get 1 beer free! Sweet.",
                "type": "regular",
                "price": "0.00",
                "capacity": "10",
                "remaining": "10",
                "sellStartDate": "0000-00-00 00:00:00",
                "sellEndDate": "0000-00-00 00:00:00",
                "minPerOrder": "0",
                "maxPerOrder": "0",
                "feeOption": "2"
            },
            {
                "id": "1078",
                "name": "2 for 1",
                "description": "Beers for a buck get yer 2nd round free!",
                "type": "regular",
                "price": "1.00",
                "capacity": "10",
                "remaining": "10",
                "sellStartDate": "0000-00-00 00:00:00",
                "sellEndDate": "0000-00-00 00:00:00",
                "minPerOrder": "0",
                "maxPerOrder": "0",
                "feeOption": "2"
            },
            {
                "id": "1079",
                "name": "Support Local",
                "description": "Pay what you want¦ beers guaranteed! \nIf you have a preference, please leave a note.",
                "type": "regular",
                "price": "0.00",
                "capacity": "10",
                "remaining": "10",
                "sellStartDate": "0000-00-00 00:00:00",
                "sellEndDate": "0000-00-00 00:00:00",
                "minPerOrder": "0",
                "maxPerOrder": "0",
                "feeOption": "2"
            },
            {
                "id": "1080",
                "name": "Beer Flights",
                "description": "RSVP and get a sampler of the beers featured this Thirsty Thursday!",
                "type": "regular",
                "price": "0.00",
                "capacity": "10",
                "remaining": "10",
                "sellStartDate": "0000-00-00 00:00:00",
                "sellEndDate": "0000-00-00 00:00:00",
                "minPerOrder": "0",
                "maxPerOrder": "0",
                "feeOption": "2"
            }
        ]
    },
    "code": 200
}
```
