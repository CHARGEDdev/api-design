### **event/details/{id}**

Deployed on branch: `api` `dev` 

#### **Description**

Get information of a event by event's id.

#### **Method**

GET

#### **Example Preview**
```
JSON: http://api.charged.fm/event/details/2683180
XML: http://api.charged.fm/event/details/2683180.xml
```
#### **Endpoint**
```
http://api.charged.fm/event/details/{EVENT_ID}
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/event/details/2683180'
```   
#### **Example Response**
```
{
    "id": 2683180,
    "title": "New York Mets vs. Los Angeles Dodgers",
    "nickname": "Mets vs. Dodgers",
    "time": "2015-07-23 19:10:00",
    "canceled": 0,
    "url": "http://www.charged.fm/new-york-mets-tickets/new-york-mets-vs-los-angeles-dodgers/07-23-2015/citi-field/mlb/2683180",
    "details": "With a bunch of young talent, the New York Mets are looking Amazin' again!",
    "taxonomy": {
        "id": 10205,
        "category": "MLB",
        "parent": {
            "id": 102,
            "category": "Baseball",
            "parent": {
                "id": 1,
                "category": "Sports",
                "parent": null
            }
        }
    },
    "images": {
        "small": "http://media.charged.fm/photos/file_5406491ac7f59.jpg",
        "medium": "http://media.charged.fm/photos/file_5406491c19d20.jpg",
        "large": "http://media.charged.fm/photos/file_5406491b2988d.jpg"
    },
    "performers": [
        {
            "id": 313,
            "name": "New York Mets",
            "nickname": "Mets",
            "url": "http://www.charged.fm/new-york-mets-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5406491ac7f59.jpg",
                "medium": "http://media.charged.fm/photos/file_5406491c19d20.jpg",
                "large": "http://media.charged.fm/photos/file_5406491b2988d.jpg"
            },
            "taxonomy": {
                "id": "10205",
                "category": "MLB",
                "parent": {
                    "id": "102",
                    "category": "Baseball",
                    "parent": {
                        "id": "1",
                        "category": "Sports",
                        "parent": null
                    }
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            },
            "details": "With a bunch of young talent, the New York Mets are looking Amazin' again!"
        },
        {
            "id": 246,
            "name": "Los Angeles Dodgers",
            "nickname": "Dodgers",
            "url": "http://www.charged.fm/los-angeles-dodgers-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_540de8cf1dcc0.jpg",
                "medium": "http://media.charged.fm/photos/file_540de8cf898c4.jpg",
                "large": "http://media.charged.fm/photos/file_540de8cf306a7.jpg"
            },
            "taxonomy": {
                "id": "10205",
                "category": "MLB",
                "parent": {
                    "id": "102",
                    "category": "Baseball",
                    "parent": {
                        "id": "1",
                        "category": "Sports",
                        "parent": null
                    }
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            },
            "details": "Clayton Kershaw, Yasiel Puig and the rest of the Dodgers are trying to return to World Series glory. Catch all of the exciting Dodgers action this season!"
        }
    ],
    "venue": {
        "id": 21729,
        "name": "Citi Field",
        "url": "http://www.charged.fm/venue/item/21729/citi-field",
        "address": {
            "address_line1": "1 Roosevelt Avenue",
            "address_line2": "",
            "city": "Flushing",
            "state": "New York",
            "zipcode": "11354",
            "country": "United States of America"
        },
        "location": {
            "lat": 40.751935,
            "lng": -73.855571
        }
    },
    "popularity": 179,
    "counts": {
        "followers": 0,
        "broadcasts": 0
    },
    "tickets": {
        "price_lowest": 27,
        "price_highest": 779,
        "quantity": 92
    }
}
```
