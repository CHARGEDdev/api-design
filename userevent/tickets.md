### **userevent/tickets**

Deployed on branch: `evan`

#### **Description**

Get information and list tickets of a user event by user event's id.

#### **Method**

GET

#### **Example Preview**
```
JSON: http://api.evan.dev.charged.fm/userevent/tickets/1165
XML: http://api.evan.devcharged.fm/userevent/tickets/1165.xml
```
#### **Endpoint**
```
http://api.evan.dev.charged.fm/userevent/tickets/{EVENT_ID}
```
#### **Example Request**
```
$ curl 'http://api.evan.dev.charged.fm/userevent/tickets/1165'
```
#### **Example Response**
```
{
  status: "success",
  data: [
    {
      id: "2442",
      name: "General Admission",
      description: "",
      type: "regular",
      price: "10.00",
      capacity: "1000",
      remaining: "995",
      sellStartDate: "0000-00-00 00:00:00",
      sellEndDate: "0000-00-00 00:00:00",
      minPerOrder: "0",
      maxPerOrder: "0",
      feeOption: "1"
    },
    {
      id: "2443",
      name: "VIP Access",
      description: "",
      type: "regular",
      price: "25.00",
      capacity: "1000",
      remaining: "995",
      sellStartDate: "0000-00-00 00:00:00",
      sellEndDate: "0000-00-00 00:00:00",
      minPerOrder: "0",
      maxPerOrder: "0",
      feeOption: "1"
    }
  ],
  code: 200
}
```
