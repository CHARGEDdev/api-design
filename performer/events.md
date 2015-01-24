### **Performer/Events**

Deployed on branch: `api`

#### **Description**

Get profile and list events of a performer by performer's id.

#### **Method**
GET

#### **Parameters**

- offset: Optional. Default 0. Offset of events listing.
- limit: Optional. Default 10. Limit the num of listed events.

#### **Example Preview**
```
JSON: http://api.charged.fm/performer/events/id/307
XML: http://api.charged.fm/performer/events/id/307.xml
```
#### **Endpoint**
```
http://api.charged.fm/performer/events/id/{PERFORMER_ID}
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/performer/events/id/307?limit=3&offset=0'
```        
#### **Example Response**
```
{
  id: 307,
  name: "Brooklyn Nets",
  url: "http://www.charged.fm/performer/item/307/brooklyn-nets",
  images: {
    small: "http://media.charged.fm/photos/file_50649189ab8d3.jpg",
    medium: "http://media.charged.fm/photos/file_50649189c85c1.jpg",
    large: "http://media.charged.fm/photos/file_50649189b35d6.jpg"
  },
  events: {
    total: 44,
    offset: 0,
    limit: 3,
    data: [
      {
        id: 2295043,
        title: "Brooklyn Nets at Atlanta Hawks",
        time: 1358382600,
        url: "http://www.charged.fm/event/item/2295043/brooklyn-nets-at-atlanta-hawks",
        performers: [
          {
            id: 32,
            name: "Atlanta Hawks",
            url: "http://www.charged.fm/performer/item/32/atlanta-hawks",
            images: {
              small: "http://media.charged.fm/photos/file_4e5fcd2593564.jpg",
              medium: "http://media.charged.fm/photos/file_4e5fcd25b6fb4.jpg",
              large: "http://media.charged.fm/photos/file_4e5fcd259dd5f.jpg"
            }
          },
          {
            id: 307,
            name: "Brooklyn Nets",
            url: "http://www.charged.fm/performer/item/307/brooklyn-nets",
            images: {
              small: "http://media.charged.fm/photos/file_50649189ab8d3.jpg",
              medium: "http://media.charged.fm/photos/file_50649189c85c1.jpg",
              large: "http://media.charged.fm/photos/file_50649189b35d6.jpg"
            }
          }
        ],
        venue: {
          id: 8908,
          name: "Philips Arena",
          url: "http://www.charged.fm/venue/item/8908/philips-arena",
          address: {
            address_line1: "One Philips Dr",
            address_line2: "",
            city: "Atlanta",
            state: "Georgia",
            country: "United States of America",
            zipcode: "30303"
          },
          location: {
            lat: "33.757796",
            lng: "-84.394569"
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
        id: 2314045,
        title: "Brooklyn Nets at New York Knicks",
        time: 1358800200,
        url: "http://www.charged.fm/event/item/2314045/brooklyn-nets-at-new-york-knicks",
        performers: [
          {
            id: 312,
            name: "New York Knicks",
            url: "http://www.charged.fm/performer/item/312/new-york-knicks",
            images: {
              small: "http://media.charged.fm/photos/file_4cf550891f174.jpg",
              medium: "http://media.charged.fm/photos/file_4cf5508942104.jpg",
              large: "http://media.charged.fm/photos/file_4cf550896da61.jpg"
            }
          },
          {
            id: 307,
            name: "Brooklyn Nets",
            url: "http://www.charged.fm/performer/item/307/brooklyn-nets",
            images: {
              small: "http://media.charged.fm/photos/file_50649189ab8d3.jpg",
              medium: "http://media.charged.fm/photos/file_50649189c85c1.jpg",
              large: "http://media.charged.fm/photos/file_50649189b35d6.jpg"
            }
          }
        ],
        venue: {
          id: 6832,
          name: "Madison Square Garden",
          url: "http://www.charged.fm/venue/item/6832/madison-square-garden",
          address: {
            address_line1: "4 Penn Plaza",
            address_line2: "",
            city: "New York",
            state: "New York",
            country: "United States of America",
            zipcode: "10001"
          },
          location: {
            lat: "40.75134538747298",
            lng: "-73.99377589338587"
          }
        }
      }
    ]
  }
}
```
