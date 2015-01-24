### **Ticket/CheckIn**

Deployed on branch: `api`

#### **Description**

Post ticket info to check in this ticket

#### **Method**
POST

#### **Parameters**
- ticketid
- qty

#### **Example Preview**
```
JSON: http://api.charged.fm/ticket/checkin/
XML: http://api.charged.fm/ticket/checkin/
```
#### **Endpoint**
```
http://api.charged.fm/ticket/checkin/
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/ticket/checkin/'
```    
#### **Example Response**
```
{
  "status": "success"
}
```
