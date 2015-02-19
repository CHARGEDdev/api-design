### **event/broadcasts/{eventID}**

Deployed on branch: `api` `dev`

#### **Description**

Returns all the broadcasts for an event

#### **Method**

GET

#### **Param**

- `access_token`
- `eventID`: the event id (required)
- `offset`: default 0
- `limit`: default 10

Example:
http://api.dev.charged.fm/event/broadcasts/2739180

```javascript
{
    limit: 10,
    offset: 0,
    totalBroadcasts: 1,
    event: {
        id: "2739180",
        name: "NBA All Star Practice",
        type: "event",
        venue: {
            id: "6832",
            name: "Madison Square Garden",
            url: "",
            address: {
                address_line1: "4 Pennsylvania Plaza",
                address_line2: "",
                city: "New York",
                state: "New York",
                zipcode: "10001",
                country: "United States of America"
            },
            position: {
                lat: "40.75041426733800",
                lng: "-73.99343736613160"
            }
        },
        date: "2015-02-14T10:30:00-05:00",
        performers: [
            {
                id: "8556",
                name: "NBA All Star Practice",
                url: "http://www.charged.fm/nba-all-star-practice-tickets"
            },
            {
                id: "2710",
                name: "NBA All Star Game",
                url: "http://www.charged.fm/nba-all-star-game-tickets"
            }
        ]
    },
    broadcasts: [
        {
            id: "190",
            caption: "All star night",
            totalLikes: "0",
            totalComments: "0",
            dateCreated: "2015-02-14T20:51:13-05:00",
            user: {
                id: "43924",
                fullName: "Gaotang Shen",
                displayName: "GTA"
            },
            images: {
                thumbnail: {
                    width: "150",
                    height: "150",
                    url: "http://media.charged.fm/photos/usergen/broadcasts/1423965072_U1juvN7x_thumbnail.jpg"
                },
                standard: {
                    width: "640",
                    height: "640",
                    url: "http://media.charged.fm/photos/usergen/broadcasts/1423965072_U1juvN7x_standard.jpg"
                },
                full: {
                    width: "960",
                    height: "960",
                    url: "http://media.charged.fm/photos/usergen/broadcasts/1423965072_U1juvN7x_full.jpg"
                }
            }
        }
    ]
}
```
