### **event**

Deployed on branch: `api`

#### **Description**

Get information of a event by event's id.

#### **Method**

GET

#### **Param**

**POST**

Example Preview
JSON: http://api.charged.fm/event/view/id/2358508
XML: http://api.charged.fm/event/view/id/2358508.xml

Endpoint
http://api.charged.fm/event/view/id/{EVENT_ID}

Example Request
$ curl 'http://api.charged.fm/event/view/id/2358508'
        
Example:

```javascript
{
  id: 2360407,
  title: "Sleep No More",
  time: 1358485200,
  url: "http://www.charged.fm/event/item/2360407/sleep-no-more",
  performers: [
    {
      id: 33669,
      name: "Sleep No More",
      url: "http://www.charged.fm/performer/item/33669/sleep-no-more",
      images: {
        small: null,
        medium: null,
        large: null
      }
    }
  ],
  venue: {
    id: 18884,
    name: "The Mckittirck Hotel",
    url: "http://www.charged.fm/venue/item/18884/the-mckittirck-hotel",
    address: {
      address_line1: "530 W.27th St.",
      address_line2: "",
      city: "New York",
      state: "New York",
      country: "United States of America",
      zipcode: "10001"
    },
    location: {
      lat: "40.7507367",
      lng: "-74.0037921"
    }
  }
}
```
