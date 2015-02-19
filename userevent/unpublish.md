### **userevent/unpublish/{id}**

Deployed on branch: `api` | `dev`

#### **Description**

Unpublish a userevent that is currently published

#### **Method**

GET

#### **Param**

- `access_token`: your access token required
- `id`: the userevent id, required
- `limit`: default 10
- `param`: explanation of param

#### **Response**

Example response

```javascript
{
    "status": "success",
    "data": {
        "id": "2118",
        "userID": "3",
        "title": "SXNY",
        "description": "South By New York",
        "image": "http://media.charged.fm/photos/file_5423a7adb5e3f.jpg",
        "startDate": "2015-03-01 19:15:00",
        "endDate": "0000-00-00 00:00:00",
        "venue": {
            "name": "CHARGED.fm",
            "address": {
                "address_line1": "",
                "address_line2": "",
                "city": "New York",
                "state": "NY",
                "zipcode": "10017",
                "country": "United States"
            },
            "location": {
                "lat": 0,
                "lng": 0
            }
        },
        "tags": "",
        "category": "1",
        "subcategory": "0",
        "public": 1,
        "url": "http://www.charged.fm/userevent/item/2118",
        "created": "0000-00-00 00:00:00",
        "published": "0",
        "datePublished": "2015-02-19 13:03:51",
        "updated": "2015-02-19 13:07:27",
        "tickets": []
    },
    "code": 200
}
```
