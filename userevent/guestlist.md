### **userevent/guestlist**

Deployed on branch: `api`

#### **Description**

List guest of a userevent by usereventid

#### **Method**

GET

#### **Endpoint**
```
http://api.charged.fm/userevent/guestlist/id/{EVENT_ID}
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/userevent/guestlist/id/792'
```      
#### **Example Response**
```
{
  "id": 792,
  "title": "The Best of Broadway",
  "time": 1359684000,
  "url": "http:\/\/www.charged.fm\/userevent\/item\/792\/the-best-of-broadway",
  "performer": "",
  "venue": {
    "name": "The Broadway Comedy Club",
    "address": {
      "address_line1": "318 W. 53rd St.",
      "address_line2": "",
      "city": "New York",
      "state": "New York",
      "country": "United States",
      "zipcode": "10019"
    },
    "location": {
      "lat": "",
      "lng": ""
    }
  },
  "guestlist": {
    "total": 100,
    "offset": 0,
    "limit": 10,
    "checkedin": 32,
    "data": [
      {
        "first_name": "Hello",
        "last_name": "Json",
        "email_address": "hello@example.com,
        "order_num": "11301398549",
        "card_type": "VISA",
        "ticket_name": "Gerneral Admission",
        "qty": 3,
        "checkedin": 1,
      },
      {
        "first_name": "Hello2",
        "last_name": "Json",
        "email_address": "hello@example.com,
        "order_num": "11301398548",
        "card_type": "VISA",
        "ticket_name": "Gerneral Admission",
        "qty": 3,
        "checkedin": 2,
      },
      {
        "first_name": "Hello3",
        "last_name": "Json",
        "email_address": "hello@example.com,
        "order_num": "11301398544",
        "card_type": "VISA",
        "ticket_name": "Gerneral Admission",
        "qty": 3,
        "checkedin": 3,
      }
    ]
  }
}
```
