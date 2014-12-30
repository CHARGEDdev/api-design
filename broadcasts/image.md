### **broadcast**

Deployed on branch: `api`, `dev`

#### **Description**
Upload an image for an event broadcast and add an optional caption

#### **Method**

POST

#### **Param**

**POST**
- access_token
- eventType [event|userevent]
- eventID
- caption
- image `FILE` Mime-type "image/jpeg", "image/png"


Example:

http://api.charged.fm/broadcast

```javascript
{
    "status":"success",
    "code":200,
    "broadcastID":18,
    "userID":2521,
    "eventID":113429,
    "eventType":"event",
    "caption":"Here's a caption dude!",
    "images":[
        "thumbnail: {
          "url": "http://media.charged.fm/photos/usergen/broadcasts/1419975648_peugwu8Q_thumbnail.jpg"
          "width": 150
          "height": 150
        }-
        "standard": {
          "url": "http://media.charged.fm/photos/usergen/broadcasts/1419975648_peugwu8Q_standard.jpg"
          "width": 640
          "height": 640
        }-
        "full": {
          "url": "http://media.charged.fm/photos/usergen/broadcasts/1419975648_peugwu8Q_full.jpg"
          "width": 960
          "height": 960
        }
      ],
    "dateCreated":"2014-12-30T16:44:11-05:00"
}
```

<hr>

### **broadcast/{broadcastID}**

Deployed on branch: `api`, `dev`

#### **Description**
Modify the caption on a broadcast

#### **Method**

PUT

#### **Param**

- access_token
- broadcastID
- caption


Example:

http://api.charged.fm/broadcast/18

```javascript
{
    "status":"success",
    "broadcastID":18,
    "caption":"Here's an updated caption yo!",
    "dateModified":"2014-12-30T16:48:54-05:00",
    "code":200
}
```

<hr>

### **broadcast/{broadcastID}**

Deployed on branch: `api`, `dev`

#### **Description**
Delete a broadcast

#### **Method**

DELETE

#### **Param**

- access_token
- broadcastID


Example:

http://api.charged.fm/broadcast/18

```javascript
{
    "status":"success",
    "broadcastID":18,
    "dateDeleted":"2014-12-30T16:52:34-05:00",
    "code":200
}
```
