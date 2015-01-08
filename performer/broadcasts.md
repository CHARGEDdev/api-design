### **performer/broadcasts/{performerID}**

Deployed on branch: `dev`

#### **Description**

Returns all the broadcasts for the performer

#### **Method**

GET

#### **Param**

- access_token
- offset: default 0
- limit: default 10

Example:
http://api.dev.charged.fm/performer/broadcasts/{performerID}52954

```javascript
{
    "limit": 10,
    "offset": 0,
    "totalBroadcasts": 0,
    "broadcasts": [
        {
            "id": "17",
            "caption": "Say WHAT?!",
            "totalLikes": "0",
            "totalComments": "0",
            "dateCreated": "2014-12-30T16:40:49-05:00",
            "images": {
                "thumbnail": {
                    "width": "150",
                    "height": "150",
                    "url": "1419975648_peugwu8Q_thumbnail.jpg"
                },
                "standard": {
                    "width": "640",
                    "height": "640",
                    "url": "1419975648_peugwu8Q_standard.jpg"
                },
                "full": {
                    "width": "960",
                    "height": "960",
                    "url": "1419975648_peugwu8Q_full.jpg"
                }
            },
            "event": {
                "eventID": "2724379",
                "performers": [
                    {
                        "performerID": "55241",
                        "performerName": "The Cadillac Three",
                        "performerSlug": "the-cadillac-three"
                    },
                    {
                        "performerID": "52954",
                        "performerName": "Brandy Clark",
                        "performerSlug": "brandy-clark"
                    },
                    {
                        "performerID": "98689",
                        "performerName": "Farmborough Festival",
                        "performerSlug": ""
                    },
                    {
                        "performerID": "53260",
                        "performerName": "Ashley Monroe",
                        "performerSlug": "ashley-monroe"
                    },
                    {
                        "performerID": "2543",
                        "performerName": "Luke Bryan",
                        "performerSlug": "luke-bryan"
                    },
                    {
                        "performerID": "1253",
                        "performerName": "Dwight Yoakam",
                        "performerSlug": "dwight-yoakam"
                    },
                    {
                        "performerID": "41605",
                        "performerName": "Kip Moore",
                        "performerSlug": "kip-moore"
                    },
                    {
                        "performerID": "96865",
                        "performerName": "Maddie & Tae",
                        "performerSlug": "maddie-tae"
                    },
                    {
                        "performerID": "3867",
                        "performerName": "Randy Houser",
                        "performerSlug": "randy-houser"
                    },
                    {
                        "performerID": "140",
                        "performerName": "Dierks Bentley",
                        "performerSlug": "dierks-bentley"
                    },
                    {
                        "performerID": "16459",
                        "performerName": "Wade Bowen",
                        "performerSlug": "wade-bowen"
                    },
                    {
                        "performerID": "45774",
                        "performerName": "Brad Paisley",
                        "performerSlug": "brad-paisley"
                    }
                ],
                "city": "New York",
                "date": "2015-06-26 03:30:00",
                "stateProvince": "NY",
                "name": "Farmborough Festival: Luke Bryan, Brad Paisley & Dierks Bentley - 3 Day Pass",
                "venue": "Randalls Island"
            }
        }
    ]
}
```
