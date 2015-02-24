### media/images

Deployed on branch: `dev`

#### **Description**

Lists all of user's uploaded images in their media library

#### **Method**

GET

#### **Param**

- `access_token`: your access token, (required)
- `offset`: default 0, (optional)
- `limit`: default 10, (optional)

Example:

```javascript

{
    "status": "success",
    "total": 5,
    "limit": 10,
    "offset": 0,
    "images": [
        {
            "id": "15",
            "name": "Screen Shot 2014-03-18 at 10.47.48 AM.png",
            "images": {
                "thumbnail": {
                    "url": "http://media.charged.fm/photos/usergen/events/thumbnail_1423598641_9zf5UyEF.png",
                    "width": "79",
                    "height": "80"
                },
                "standard": {
                    "url": "http://media.charged.fm/photos/usergen/events/standard_1423598641_9zf5UyEF.png",
                    "width": "599",
                    "height": "600"
                },
                "original": {
                    "url": "http://media.charged.fm/photos/usergen/events/1423598641_9zf5UyEF.png",
                    "width": "1391",
                    "height": "1393"
                }
            },
            "dateCreated": "2015-02-10T15:04:02-05:00"
        }
    ],
    "code": 200
}
```
