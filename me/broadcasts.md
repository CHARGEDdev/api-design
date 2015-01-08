### **me/broadcasts**

Deployed on branch: `api` `dev`

#### **Description**

Returns all the broadcasts for the logged in user

#### **Method**

GET

#### **Param**

- access_token
- offset: default 0
- limit: default 10

Example:
http://api.charged.fm/me/broadcasts

```javascript

{
    "limit": 10,
    "offset": 0,
    "totalBroadcasts": 3,
    "broadcasts": [
        {
            "id": "19",
            "caption": "Here's+a+caption%2Bdude1%2B",
            "totalLikes": "0",
            "totalComments": "0",
            "dateCreated": "2014-12-30T17:04:29-05:00",
            "images": {
                "thumbnail": {
                    "width": "150",
                    "height": "150",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977069_oHMJrteD_thumbnail.jpg"
                },
                "standard": {
                    "width": "640",
                    "height": "640",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977069_oHMJrteD_standard.jpg"
                },
                "full": {
                    "width": "960",
                    "height": "960",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977069_oHMJrteD_full.jpg"
                }
            },
            "event": {
                "usereventid": "23",
                "title": "DJ Jake's Hip-Hop Spectacular",
                "startDate": "2011-08-01 10:30 PM",
                "venueName": "The Palace",
                "host": "Jake",
                "userID": "97",
                "username": "jake.langbecker@gmail.com",
                "displayName": "langbecker",
                "fullName": "Jake Langbecker",
                "eventType": "userevent"
            }
        },
        {
            "id": "20",
            "caption": "Test+Caption+here's%2Ba%2Bplus+sign",
            "totalLikes": "0",
            "totalComments": "0",
            "dateCreated": "2014-12-30T17:08:39-05:00",
            "images": {
                "thumbnail": {
                    "width": "150",
                    "height": "150",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977318_38yexH15_thumbnail.jpg"
                },
                "standard": {
                    "width": "640",
                    "height": "640",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977318_38yexH15_standard.jpg"
                },
                "full": {
                    "width": "960",
                    "height": "960",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1419977318_38yexH15_full.jpg"
                }
            },
            "event": {
                "eventID": "2613030",
                "performers": [
                    {
                        "performerID": "314",
                        "performerName": "New York Rangers",
                        "performerSlug": "new-york-rangers"
                    },
                    {
                        "performerID": "310",
                        "performerName": "New York Islanders",
                        "performerSlug": "new-york-islanders"
                    }
                ],
                "city": "New York",
                "date": "2015-01-13 19:00:00",
                "stateProvince": "NY",
                "name": "New York Rangers vs. New York Islanders",
                "venue": "Madison Square Garden"
            }
        }
        {
            "id": "22",
            "caption": "Derpy derpy",
            "totalLikes": "0",
            "totalComments": "0",
            "dateCreated": "2015-01-06T14:22:27-05:00",
            "images": {
                "thumbnail": {
                    "width": "150",
                    "height": "150",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1420572144_CnREQnBH_thumbnail.jpg"
                },
                "standard": {
                    "width": "640",
                    "height": "640",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1420572144_CnREQnBH_standard.jpg"
                },
                "full": {
                    "width": "960",
                    "height": "960",
                    "url": "http://media.charged.fm/photos/usergen/broadcasts/1420572144_CnREQnBH_full.jpg"
                }
            },
            "event": {
                "usereventid": "23",
                "title": "DJ Jake's Hip-Hop Spectacular",
                "startDate": "2011-08-01 10:30 PM",
                "venueName": "The Palace",
                "host": "Jake",
                "userID": "97",
                "username": "jake.langbecker@gmail.com",
                "displayName": "langbecker",
                "fullName": "Jake Langbecker",
                "eventType": "userevent"
            }
        }
    ]
}
```
