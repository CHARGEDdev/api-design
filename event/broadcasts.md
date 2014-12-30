### **event/broadcasts/{eventID}**

Deployed on branch: `api` `dev`

#### **Description**

Returns all the broadcasts for an event

#### **Method**

GET

#### **Param**

- access_token
- eventID
- offset: default 0
- limit: default 10
- Paramx: simple explanation

Example:
http://api.evan.dev.charged.fm/event/broadcasts/2613002

```javascript
{
    "limit": 10,
    "offset": 0,
    "totalBroadcasts": 1,
    "event": {
        "eventID": "2613002",
        "performers": [
            {
                "performerID": "314",
                "performerName": "New York Rangers",
                "performerSlug": "new-york-rangers"
            },
            {
                "performerID": "78",
                "performerName": "Buffalo Sabres",
                "performerSlug": "buffalo-sabres"
            }
        ],
        "city": "New York",
        "date": "2015-01-03 19:00:00",
        "stateProvince": "NY",
        "name": "New York Rangers vs. Buffalo Sabres",
        "venue": "Madison Square Garden"
    },
    "broadcasts": [
        {
            "id": "21",
            "caption": "Here's a motherfucking caption+ya+bish",
            "totalLikes": "0",
            "totalComments": "0",
            "dateCreated": "2014-12-30T17:12:06-05:00",
            "user": {
                "id": "113429",
                "fullName": "Evan Ridenour",
                "displayName": "evride"
            },
            "images": {
                "thumbnail": {
                    "width": "150",
                    "height": "150",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977525_004uDQth_thumbnail.jpg"
                },
                "standard": {
                    "width": "640",
                    "height": "640",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977525_004uDQth_standard.jpg"
                },
                "full": {
                    "width": "960",
                    "height": "960",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977525_004uDQth_full.jpg"
                }
            }
        }
    ]
}
```
