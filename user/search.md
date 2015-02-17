### **user/search**

Deployed on branch: `api` `dev`

#### **Description**

Search for any user using a query string, plus any of the optional parameters below

#### **Method**

GET

#### **Param**

- `q`: search terms
- `username`: a username, without the '@' prepended 
- `first_name`: first name of user
- `last_name`: last name of user
- `offset`: pagination offset
- `limit`: pagination size limit

Examples:
* http://api.dev.charged.fm/user/search?email=henrik@charged.fm
* http://api.dev.charged.fm/user/search?first_name=henrik&last_name=r
* http://api.gt.dev.charged.fm/user/search?username=h

```javascript
{
    "total": 1,
    "offset": 0,
    "limit": 1,
    "data": [
        {
            "id": "3",
            "username": "h",
            "first_name": "Henrik",
            "last_name": " R",
            "images": {
                "small": "http://media.charged.fm/media/file_4e28670f9c3bf.jpg",
                "medium": "http://media.charged.fm/media/file_4e28670fa2180.jpg",
                "large": "http://media.charged.fm/media/file_4e28670f66496.jpg"
            }
        }
    ]
}
```
