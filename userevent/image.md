### **userevent/image**

Deployed on branch: `evan`

#### **Description**

Set an image for the userevent

#### **Method**

POST

#### **Param**

- access_token
- mediaID (Upload image using the media/image endpoint and pass in the mediaID you get back)

Example:

```javascript
{
    "status": "success",
    "data": {
        "id": "2000",
        "userID": "113429",
        "title": "derpz",
        "description": "HERROZ!",
        "image": "standard_1422528569_UF",
        "startDate": "0000-00-00 00:00:00",
        "endDate": "0000-00-00 00:00:00",
        "venue": {
            "name": "",
            "address": {
                "address": "",
                "city": "",
                "state": "",
                "zipcode": "",
                "country": ""
            },
            "coordinates": {
                "latitude": "",
                "longitude": ""
            }
        },
        "tags": "",
        "category": "0",
        "subcategory": "0",
        "public": "yes",
        "url": "2000",
        "created": "0000-00-00 00:00:00",
        "published": "0000-00-00 00:00:00",
        "updated": "2015-02-10 09:27:31",
        "tickets": [
            {
                "id": "3945",
                "name": "",
                "description": "",
                "type": "regular",
                "price": "0.00",
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
    "code": 200
}
```
