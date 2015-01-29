### **media/image/**

Deployed on branch: `dev`

#### **Description**

Uploads an image to the users media library

#### **Method**

POST

#### **Param**

- access_token
- image FILE

Example:

http://api.dev.charged.fm/media/image

```javascript
{
    "status": "success",
    "mediaID": 12,
    "name": "1527122_10203703648409394_5591148675519717190_n.jpg",
    "images": {
        "thumbnail": {
            "url": "http://media.charged.fm/photos/usergen/events/thumbnail_1422528127_6GDOVimU.jpg",
            "width": 106,
            "height": 80
        },
        "standard": {
            "url": "http://media.charged.fm/photos/usergen/events/standard_1422528127_6GDOVimU.jpg",
            "width": 800,
            "height": 600
        },
        "original": {
            "url": "http://media.charged.fm/photos/usergen/events/original_1422528127_6GDOVimU.jpg",
            "width": 4000,
            "height": 3000
        }
    },
    "dateCreated": "2015-01-29T05:42:07-05:00",
    "code": 201
}
```




### **media/image/{id}**

Deployed on branch: `dev`

#### **Description**

Delete user's media library image

#### **Method**

DELETE

#### **Param**

- access_token

Example:

http://api.dev.charged.fm/media/image/12
```javascript
{
    "status": "success",
    "id": 12,
    "code": 200
}
```
