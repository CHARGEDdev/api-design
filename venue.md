### **Venue**

Deployed on branch: `api`

#### **Description**

Get infomation of a venue by venue's id.

#### **Method**
GET

#### **Example Preview**
```
JSON: http://api.charged.fm/venue/view/id/20182
XML: http://api.charged.fm/venue/view/id/20182.xml
```
#### **Endpoint**
```
http://api.charged.fm/venue/view/id/{VENUE_ID}
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/venue/view/id/20182'
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
  }
}
```
