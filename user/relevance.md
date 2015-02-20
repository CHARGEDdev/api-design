### **user/relevance/{uid}**

Deployed on branch: `gt`

#### **Description**

#### **Method**

Get

#### **Param**

- `uid`: user id (required)
- `access_token`: your access token (required)

Example:

http://api.gt.dev.charged.fm/user/relevance/43924

```javascript
{
    "id": 43924,
    "username": "GTA",
    "email": "gaotang@charged.fm",
    "fullname": "Gaotang Shen",
    "gender": "Male",
    "birthday": "0000-00-00",
    "biography": "",
    "avatar": "http://media.charged.fm/media/file_5334b363c6bd0.jpg",
    "thumb": "http://media.charged.fm/media/file_5334b364043a8.jpg",
    "relevance": {
        "score": 21,
        "points": [
            {
                "ticket_purchase": 5,       //purchasing a ticket
                "ticket_sale": 5,           //selling a ticket
                "userevent_rsvp": 1,        //somebody RSVPs to your event
                "userevent_broadcast": 2,   //somebody broadcasts your event
                "event_broadcast": 1,       //you broadcast an event
                "event_broadcast_like": 1,  //somebody likes your broadcast
                "me_follow": 1,             //somebody follows you
                "me_connect": 2,            //connecting a social media account
                "me_account": 3             //signing up
            }
        ]
    }
}
```
