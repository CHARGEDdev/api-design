### **userevent/publish/{id}**

Deployed on branch: `api` | `dev`

#### **Description**

Publish a userevent that is currently unpublished

#### **Method**

GET

#### **Param**

- `access_token`: your access token required
- `id`: the userevent id, required
- `limit`: default 10
- `param`: explanation of param

Parameters to ensure the userevent is ready to be published, otherwise it will return an error response:

- **`title`**: title of event (required)
- **`description`**: decription of event (required)
- **`startDate`**: day event starts - YYYY-MM-DD HH:MM:SS - (required) and must be date/time in the future
- **`venueName`**: venue name - String (required)
- **`city`**: name of city - String (required) 
- *`state`*:  name of state - String (optional, but required if "United States")
- *`zipcode`*: integer (optional, but required if "United States")
- **`country`**: name of country, eg. "United States" (required) 
- **`category`**: category id (required)

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
        "public": "yes",
        "url": "2118",
        "created": "0000-00-00 00:00:00",
        "published": "2015-02-19 13:03:51",
        "updated": "2015-02-19 13:03:51",
        "tickets": []
    },
    "code": 200
}
```
