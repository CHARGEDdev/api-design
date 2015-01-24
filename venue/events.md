### **Venue/Events**

Deployed on branch: `api`

#### **Description**

Get infomation and list events of a venue by venue's id.

#### **Method**
GET

#### **Parameters**
- offset: Optional. Default 0. Offset of events listing.
- limit: Optional. Default 10. Limit the num of listed events.

#### **Example Preview**
```
JSON: http://api.charged.fm/venue/events/id/20182
XML: http://api.charged.fm/venue/events/id/20182.xml
```
#### **Endpoint**
```
http://api.charged.fm/venue/events/id/{VENUE_ID}
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/venue/events/id/20182?limit=3&offset=0'
```
#### **Example Response**
```
{
  id: 20182,
  name: "Barclays Center",
  url: "http://www.charged.fm/venue/item/20182/barclays-center",
  address: {
    address_line1: "Atlantic Avenue",
    address_line2: "",
    city: "Brooklyn",
    state: "New York",
    country: "United States of America",
    zipcode: "11217"
  },
  location: {
    lat: "40.681866782543686",
    lng: "-73.97572288844742"
  },
  events: {
    total: 73,
    offset: 0,
    limit: 3,
    data: [
      {
        id: 2294974,
        title: "Green Day",
        time: 1358384400,
        url: "http://www.charged.fm/event/item/2294974/green-day",
        performers: [
          {
            id: 183,
            name: "Green Day",
            url: "http://www.charged.fm/performer/item/183/green-day",
            images: {
              small: "http://media.charged.fm/photos/file_4fa2ac1321c76.jpg",
              medium: "http://media.charged.fm/photos/file_4fa2ac1479aa1.jpg",
              large: "http://media.charged.fm/photos/file_4fa2ac13ba1e9.jpg"
            }
          }
        ],
        venue: {
          id: 20182,
          name: "Barclays Center",
          url: "http://www.charged.fm/venue/item/20182/barclays-center",
          address: {
            address_line1: "Atlantic Avenue",
            address_line2: "",
            city: "Brooklyn",
            state: "New York",
            country: "United States of America",
            zipcode: "11217"
          },
          location: {
            lat: "40.681866782543686",
            lng: "-73.97572288844742"
          }
        }
      },
      {
        id: 2296005,
        title: "Atlanta Hawks at Brooklyn Nets",
        time: 1358555400,
        url: "http://www.charged.fm/event/item/2296005/atlanta-hawks-at-brooklyn-nets",
        performers: [
          {
            id: 307,
            name: "Brooklyn Nets",
            url: "http://www.charged.fm/performer/item/307/brooklyn-nets",
            images: {
              small: "http://media.charged.fm/photos/file_50649189ab8d3.jpg",
              medium: "http://media.charged.fm/photos/file_50649189c85c1.jpg",
              large: "http://media.charged.fm/photos/file_50649189b35d6.jpg"
            }
          },
          {
            id: 32,
            name: "Atlanta Hawks",
            url: "http://www.charged.fm/performer/item/32/atlanta-hawks",
            images: {
              small: "http://media.charged.fm/photos/file_4e5fcd2593564.jpg",
              medium: "http://media.charged.fm/photos/file_4e5fcd25b6fb4.jpg",
              large: "http://media.charged.fm/photos/file_4e5fcd259dd5f.jpg"
            }
          }
        ],
        venue: {
          id: 20182,
          name: "Barclays Center",
          url: "http://www.charged.fm/venue/item/20182/barclays-center",
          address: {
            address_line1: "Atlantic Avenue",
            address_line2: "",
            city: "Brooklyn",
            state: "New York",
            country: "United States of America",
            zipcode: "11217"
          },
          location: {
            lat: "40.681866782543686",
            lng: "-73.97572288844742"
          }
        }
      },
      {
        id: 2314508,
        title: "Disney On Ice: Treasure Trove",
        time: 1358985600,
        url: "http://www.charged.fm/event/item/2314508/disney-on-ice-treasure-trove",
        performers: [
          {
            id: 797,
            name: "Disney On Ice",
            url: "http://www.charged.fm/performer/item/797/disney-on-ice",
            images: {
              small: "http://media.charged.fm/photos/file_4c2124bf9210b.jpg",
              medium: "http://media.charged.fm/photos/file_4c2124bfaaf7e.jpg",
              large: "http://media.charged.fm/photos/file_4c2124bfc8ffb.jpg"
            }
          }
        ],
        venue: {
          id: 20182,
          name: "Barclays Center",
          url: "http://www.charged.fm/venue/item/20182/barclays-center",
          address: {
            address_line1: "Atlantic Avenue",
            address_line2: "",
            city: "Brooklyn",
            state: "New York",
            country: "United States of America",
            zipcode: "11217"
          },
          location: {
            lat: "40.681866782543686",
            lng: "-73.97572288844742"
          }
        }
      }
    ]
  }
}
```
