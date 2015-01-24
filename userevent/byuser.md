### **Userevent/ByUser**

Deployed on branch: `api`

#### **Description**

List userevents by user id.

#### **Method**
GET

#### **Parameters**
- offset: Optional. Default 0. Offset of userevents to be listed.
- limit: Optional. Default 10. Limit the num of userevents to be listed.
- year: Optional. No Default. Year of userevents to be listed.
- month: Optional. No Default. Month of userevents to be listed.
- keyword: Optional. No Default. Search keyword of userevents to be listed.

#### **Example Preview**
JSON: http://api.charged.fm/userevent/user/uid/{User_ID}
XML: http://api.charged.fm/userevent/user/uid/{User_ID}.xml

#### **Endpoint**
http://api.charged.fm/userevent/user/uid/{User_ID}

#### **Example Request**
$ curl 'http://api.charged.fm/userevent/user/uid/{User_ID}'
        
#### **Example Response**
```
{
  "userid": 100,
  "username": "myname",
  "avatar": "http://www.charged.fm/avatar/avatar.jpg"
  "total": 22,
  "offset": 0,
  "limit": 10,
  "year": 2013,
  "month": 01,
  "data": [
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
      }
    },
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
      }
    }
  ]
}
```
