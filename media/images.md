### *media/images**

Deployed on branch: `dev`

#### **Description**

Lists all of user's uploaded images

#### **Method**

GET

#### **Param**

- access_token
- offset: default 0
- limit: default 10

Example:

```javascript

{
    "status": "success",
    "total": 2,
    "limit": 10,
    "offset": 0
    "images": [
        {
            "id": "11",
            "name": "IMG_20140405_132313.jpg",
            "images": {
                "thumbnail": {
                    "url": "http://media.charged.fm/photos/usergen/events/thumbnail_1422504370_zmnobOnr.jpg",
                    "width": "106",
                    "height": "80"
                },
                "standard": {
                    "url": "http://media.charged.fm/photos/usergen/events/standard_1422504370_zmnobOnr.jpg",
                    "width": "800",
                    "height": "600"
                },
                "original": {
                    "url": "http://media.charged.fm/photos/usergen/events/original_1422504370_zmnobOnr.jpg",
                    "width": "4000",
                    "height": "3000"
                }
            },
            "dateCreated": "2015-01-28T23:06:10-05:00"
        },
        {
            "id": "13",
            "name": "1527122_10203703648409394_5591148675519717190_n.jpg",
            "images": {
                "thumbnail": {
                    "url": "http://media.charged.fm/photos/usergen/events/thumbnail_1422528569_UF2hGsvt.jpg",
                    "width": "106",
                    "height": "80"
                },
                "standard": {
                    "url": "http://media.charged.fm/photos/usergen/events/standard_1422528569_UF2hGsvt.jpg",
                    "width": "800",
                    "height": "600"
                },
                "original": {
                    "url": "http://media.charged.fm/photos/usergen/events/1422528569_UF2hGsvt.jpg",
                    "width": "960",
                    "height": "720"
                }
            },
            "dateCreated": "2015-01-29T05:49:29-05:00"
        }
    ],
    "code": 200
}
```
