### **userevent/tickets**

Deployed on branch: `api`

#### **Description**

Get information and list tickets of a user event by user event's id.

#### **Method**

GET

#### **Param**

Example Preview
JSON: http://api.charged.fm/userevent/tickets/id/792
XML: http://api.charged.fm/userevent/tickets/id/792.xml

Endpoint
http://api.charged.fm/userevent/tickets/id/{EVENT_ID}

Example Request
$ curl 'http://api.charged.fm/userevent/tickets/id/792'

Example:

```javascript
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
  "tickets": [
    {
      "id": "1765",
      "name": "General Admission",
      "price": "20.00",
      "quantity": "180"
    }
  ]
}
```
