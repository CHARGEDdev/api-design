### **userevent/ticket**

Deployed on branch: `dev`

#### **Description**

Create and update tickets

#### **Method**

PUT or POST

#### **Param**

- `access_token`

Required:
- `id` (Ticket id used to update ticket)
- `eventID` (Only needed when ticketID is not passed to the endpoint, creates ticket, is not used after ticket is created)

Optional:
- `name`
- `description`
- `type` [regular|free|donation] - defaults to regular
- `price`
- `sellStartDate` YYYY-MM-DD HH:MM:SS
- `sellEndDate` YYYY-MM-DD HH:MM:SS
- `minPerOrder`
- `maxPerOrder`
- `capacity`
- `feeOption` (Not used in app yet. ignore)



Example:
http://api.dev.charged.fm/userevent/ticket
```javascript
{
    "status": "success",
    "data": {
        "id": "3964",
        "name": "Early Bird",
        "description": "Hey",
        "type": "regular",
        "price": "10.00",
        "capacity": "100",
        "remaining": "0",
        "sellStartDate": "2015-02-20 00:00:00",
        "sellEndDate": "0000-00-00 00:00:00",
        "minPerOrder": "1",
        "maxPerOrder": "4",
        "feeOption": "1"
    },
    "code": 200
}
```




### **userevent/ticket/{id}**

Deployed on branch: `evan`

#### **Description**

Delete ticket

#### **Method**

DELETE

#### **Param**

- `access_token`
- `id`



### **userevent/ticket/{id}**

Deployed on branch: `evan`

#### **Description**

Get ticket

#### **Method**

GET

#### **Param**

- access_token
- id

Example:
http://api.evan.dev.charged.fm/userevent/ticket/3935
```javascript
{
    "status": "success",
    "data": {
        "id": "3964",
        "name": "Early Bird",
        "description": "Hey",
        "type": "regular",
        "price": "10.00",
        "capacity": "100",
        "remaining": "0",
        "sellStartDate": "2015-02-20 00:00:00",
        "sellEndDate": "0000-00-00 00:00:00",
        "minPerOrder": "1",
        "maxPerOrder": "4",
        "feeOption": "1"
    },
    "code": 200
}
```
