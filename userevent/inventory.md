### **Userevent/Inventory**

Deployed on branch: `api`

#### **Description**

load inventory of the event. 
- if If-Modified-Since is given on request, api returns only updates on the inventory tree.
- verbose :to reduce response size, we minify the key names in json. set verbose to view verbose information

#### **Method**
GET

#### **Example Preview**
```
JSON: http://api.charged.fm/userevent/inventory/{id}
XML: http://api.charged.fm/userevent/inventory/{id}
```
#### **Endpoint**
```
http://api.charged.fm/userevent/inventory/{id}
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/userevent/inventory/{id}'
$ curl 'http://api.charged.fm/userevent/inventory/{id}&verbose=1'
```        
#### **Example Response**
```
{
    "total": 5365,
    "quantity": 5339,
    "sections": [
        {
            "name": "Box Seats 01",
            "ga": false,
            "quantity": 76,
            "price_min": 0.1,
            "price_max": 50,
            "rows": [
                {
                    "name": "A",
                    "quantity": 1,
                    "price_min": 10,
                    "price_max": 10,
                    "seats": [
                        {
                            "tid": 579777,
                            "name": "1",
                            "price": 10,
                            "status": 0
                        },
                        .
                        .
                    ]
                }
                .
                .
            ]
        }
        .
        .
    ]
}
```
