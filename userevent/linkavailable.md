### **userevent/linkavailable/**

Deployed on branch: `dev`, v1.1

#### **Description**

Check to see if I link url is available

#### **Method**

GET

#### **Param**

- `access_token`: your access token required
- `name`: string, required
- `eventID`: the userevent id, optional


#### **Response**

Example response

http://api.dev.charged.fm/userevent/linkavailable?eventID=1878&name=edittest2
```javascript
{
    "name": "edittest2",
    "available": true
}
```
