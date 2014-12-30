### **POST broadcasts/image**

Deployed on branch: `dev`

#### **Description**


#### **Param**

- access_token
- eventType [event|userevent]
- eventID
- caption
- image `FILE` Mime-type "image/jpeg", "image/png"

Example:

http://api.charged.fm/broadcasts/image

```javascript
{
    "status":"success",
    "code":200,
    "broadcastID":112,
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
