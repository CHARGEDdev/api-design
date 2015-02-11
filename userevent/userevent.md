### **userevent/userevent/{id}**

Deployed on branch: `evan`

#### **Description**

Get detailed userevent information.

#### **Method**

GET

#### **Param**

- id: userevent id

Example:

http://api.evan.dev.charged.fm/userevent/userevent/459

```javascript
{
    "status": "success",
    "userevent": {
        "id": "459",
        "userID": "3",
        "title": "Thirsty Thursdays",
        "description": "<p><b>Announcing our first official Thirsty Thursday's at the new offices at CHARGED.fm</b></p><p><span style=\"line-height: 20px;\">Have a beer on us, RSVP for a sampler or just a beer or chip-in a dollar or more to get a beer or more. Or even BYOB! Whatever you do, come join us, have fun, quench your thirst after a hard day at work, and relax and enjoy the view.</span></p><p><span style=\"line-height: 20px;\"><br></span><span style=\"line-height: 20px;\">Hope to see you there!</span></p><p><span style=\"line-height: 20px;\"><br></span><span style=\"line-height: 20px;\">Henrik</span></p>",
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
                "description": "Beers for a buck â€” get yer 2nd round free!",
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
                "description": "Pay what you wantâ€¦ beers guaranteed! \nIf you have a preference, please leave a note.",
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
