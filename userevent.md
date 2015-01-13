### **userevent/create/{id}**

Deployed on branch: `api` `dev`

#### **Description**

Create new unique userevent

#### **Method**

POST

#### **Param**

**POST**

- usereventid
- title
- description
- time
- date
- venue
- host
- category
- public
- publicattendeelist
- password

Example:

```javascript
{
    "usereventid": 635,
    "title": "Bedstuy Indie Film Gathering",
    "description": "Private viewing of local independent films",
    "time": "20:00:00-05:00",
    "date": "2015-12-26",
    "venue": {
        "name": "Colador",
        "address": {
            "address_line1": "1000 Bedford Ave",
            "address_line2": "",
            "city": "Brooklyn",
            "state": "New York",
            "country": "United States",
            "zipcode": "11205"
        },
        "location": {
            "lat": "",
            "lng": ""
        }
    },
    "host": {
    	"name": Trey LaTrash,
    	"hostdescription": 
	},
    "category": {
        "subcategory": 0,
        "tags": movies, indie, under $20
    },
    "public": true,
    "public_attendee_list": true,
    "password": true
}
```
