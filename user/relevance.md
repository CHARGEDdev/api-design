### **user/relevance/{uid}**

Deployed on branch: `gt`

#### **Description**

#### **Method**

Get

#### **Param**

- `uid`: user id (required)
- `access_token`: your access token (required)

Example:

http://api.dev.charged.fm/user/relevance/43924

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
    "score": {
        "ticket_purchase": "5",
        "ticket_sale": "5",
        "userevent_rsvp": "1",
        "userevent_broadcast": "2",
        "event_broadcast": "1",
        "event_broadcast_like": "1",
        "me_follow": "1",
        "me_connect": "2",
        "me_account": "3"
    }
}
```
