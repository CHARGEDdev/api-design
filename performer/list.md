### **performer/list**

Deployed on branch: `dev`

#### **Description**

Returns all performers

#### **Method**

GET

#### **Param**

- total
- offset
- limit: 10
- data

Example:
http://api.charged.fm/performer/list

```javascript
{
    "total": 74650,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": 1,
            "name": "3",
            "url": "http://www.charged.fm/3-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423a3c650b18.jpg",
                "medium": "http://media.charged.fm/photos/file_5423a3c6935b6.jpg",
                "large": "http://media.charged.fm/photos/file_5423a3c65ba7f.jpg"
            },
            "taxonomy": {
                "id": "3",
                "category": "Theater",
                "parent": null
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 2,
            "name": "42nd Street",
            "url": "http://www.charged.fm/42nd-street-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423446421a6f.jpg",
                "medium": "http://media.charged.fm/photos/file_5423446468b21.jpg",
                "large": "http://media.charged.fm/photos/file_542344642da62.jpg"
            },
            "taxonomy": {
                "id": "306",
                "category": "Musicals",
                "parent": {
                    "id": "3",
                    "category": "Theater",
                    "parent": null
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 3,
            "name": "AFI",
            "url": "http://www.charged.fm/afi-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423a9e9dc1e7.jpg",
                "medium": "http://media.charged.fm/photos/file_5423a9ea6e195.jpg",
                "large": "http://media.charged.fm/photos/file_5423a9e9ed837.jpg"
            },
            "taxonomy": {
                "id": "202",
                "category": "Alternative",
                "parent": {
                    "id": "2",
                    "category": "Concert",
                    "parent": null
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 4,
            "name": "Aaron Lewis",
            "url": "http://www.charged.fm/aaron-lewis-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423a5ab10435.jpg",
                "medium": "http://media.charged.fm/photos/file_5423a5ab98920.jpg",
                "large": "http://media.charged.fm/photos/file_5423a5ab2a74e.jpg"
            },
            "taxonomy": {
                "id": "202",
                "category": "Alternative",
                "parent": {
                    "id": "2",
                    "category": "Concert",
                    "parent": null
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 5,
            "name": "Abba",
            "url": "http://www.charged.fm/abba-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423a08383404.jpg",
                "medium": "http://media.charged.fm/photos/file_5423a0840c9fc.jpg",
                "large": "http://media.charged.fm/photos/file_5423a0839a867.jpg"
            },
            "taxonomy": {
                "id": "218",
                "category": "Pop",
                "parent": {
                    "id": "2",
                    "category": "Concert",
                    "parent": null
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 6,
            "name": "Ema",
            "url": "http://www.charged.fm/ema-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423433703fd4.jpg",
                "medium": "http://media.charged.fm/photos/file_5423433748c1a.jpg",
                "large": "http://media.charged.fm/photos/file_542343370f965.jpg"
            },
            "taxonomy": {
                "id": "218",
                "category": "Pop",
                "parent": {
                    "id": "2",
                    "category": "Concert",
                    "parent": null
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 7,
            "name": "Aer",
            "url": "http://www.charged.fm/aer-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_542345fb58339.jpg",
                "medium": "http://media.charged.fm/photos/file_542345fbebbaa.jpg",
                "large": "http://media.charged.fm/photos/file_542345fb6c7d1.jpg"
            },
            "taxonomy": {
                "id": "202",
                "category": "Alternative",
                "parent": {
                    "id": "2",
                    "category": "Concert",
                    "parent": null
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 8,
            "name": "Aida",
            "url": "http://www.charged.fm/aida-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423a46a5f16e.jpg",
                "medium": "http://media.charged.fm/photos/file_5423a46ad8c22.jpg",
                "large": "http://media.charged.fm/photos/file_5423a46a7d116.jpg"
            },
            "taxonomy": {
                "id": "306",
                "category": "Musicals",
                "parent": {
                    "id": "3",
                    "category": "Theater",
                    "parent": null
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 9,
            "name": "Air",
            "url": "http://www.charged.fm/air-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423a1473ea2e.jpg",
                "medium": "http://media.charged.fm/photos/file_5423a147bea81.jpg",
                "large": "http://media.charged.fm/photos/file_5423a1475438f.jpg"
            },
            "taxonomy": {
                "id": "2",
                "category": "Concert",
                "parent": null
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        },
        {
            "id": 10,
            "name": "Air Supply",
            "url": "http://www.charged.fm/air-supply-tickets",
            "images": {
                "small": "http://media.charged.fm/photos/file_5423a2e684df3.jpg",
                "medium": "http://media.charged.fm/photos/file_5423a2e6cd864.jpg",
                "large": "http://media.charged.fm/photos/file_5423a2e6914df.jpg"
            },
            "taxonomy": {
                "id": "218",
                "category": "Pop",
                "parent": {
                    "id": "2",
                    "category": "Concert",
                    "parent": null
                }
            },
            "counts": {
                "followers": 0,
                "broadcasts": 0
            }
        }
    ]
}
```
