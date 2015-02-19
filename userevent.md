### **userevent**

Deployed on branch: `dev`

#### **Description**

Create new userevent. Use POST to create a userevent and a usereventid will be returned in the JSON data.
Reuse that ID in future POST and PUT calls to update the user event. All fields are optional when updating.
A "publish" endpoint will be used to publish an event and double check all data to make sure it's legit.

UPDATE: the 'id' and 'updated' properties will be removed since they'll be included in the userevent object.
Just leaving them up to keep the app working for the time being

#### **Method**

POST

#### **Param**

**POST**

- **`access_token`**: your user's access token (required)
- `id`: userevent id (ommit if creating an event, include to update existing event)
- **`title`**: title of event (required)
- **`description`**: decription of event (required)
- **`startDate`**: day event starts - YYYY-MM-DD HH:MM:SS - (required) and must be date/time in the future
- `endDate`: day event ends - YYYY-MM-DD HH:MM:SS (optional)
- `venueTBA`: venue to be announced - Boolean (optional)
- **`venueName`**: venue name - String (required)
- `venueAddress`: address of venue - String (optional)
- **`city`**: name of city - String (required) 
- *`state`*:  name of state - String (optional, but required if United States)
- *`zipcode`*: integer (optional, but required if United States)
- **`country`**: name of country, eg. "United States" (required) 
- `host`: host's username (optional)
- `hostDescription`: description of host (optional)
- **`category`**: category id (required)
- `subcategory`: subcategory id (optional)
- `tags`: tags as comma delimited string (optional)
- `displayName`: short URL, string (the string is appended to the url `www.charged.fm/<displayName>` ) (optional)
- `public`: whether event is public or private, boolean, defaults to true (optional)
- `publicAttendeeList`: whether attendee list is public or private, boolean, defaults to true (optional)
- `password`: password protect event, string (optional)

Example:

```javascript
{
    "status": "success",
    "id": 2000,
    "userevent": {
        "id": "2000",
        "userID": "113429",
        "title": "derpz",
        "description": "HERROZ!",
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
            "location": {
                "lat": "",
                "lng": ""
            }
        },
        "tags": "",
        "category": "0",
        "subcategory": "0",
        "public": "yes",
        "url": "2000",
        "created": "0000-00-00 00:00:00",
        "published": "0000-00-00 00:00:00",
        "updated": "2015-02-04 16:46:13"
    },
    "updated": "2015-02-04T16:48:12-05:00",
    "code": 200
}
```

----------------------

### **userevent/{id}**

Deployed on branch: `dev`

#### **Description**

Read the userevent data 

#### **Method**

GET

#### **Param**

- `id`: userevent id (required)
- `password`: password for userevent (optional)

Example:

```javascript
{
    "status": "success",
    "userevent": {
        "id": "1934",
        "userID": "66784",
        "title": "Dinner and a Suit on CHARGED.fm LIVE",
        "description": "<p>This is my description!</p>",
        "startDate": "2014-11-24 00:00:00",
        "endDate": "2014-11-24 00:00:00",
        "venue": {
            "name": "CHARGED.fm Studios",
            "address": {
                "address": null,
                "city": "Brooklyn",
                "state": "New York",
                "zipcode": "11201",
                "country": "United States"
            },
            "location": {
                "lat": "",
                "lng": ""
            }
        },
        "tags": "Music-Performance",
        "category": "3",
        "subcategory": "10",
        "public": "yes",
        "url": "http://www.charged.fm/userevent/item/1934",
        "created": "0000-00-00 00:00:00",
        "published": "0000-00-00 00:00:00",
        "updated": "2014-11-14 18:52:18"
    },
    "code": 200
}
```
