### **user/followingEvents/{uid}**

Deployed `dev`

#### **Method**

GET

#### **Param**

- uid
- access_token
- offset: default 0
- limit: default 10

Example:

http://api.denzel.dev.charged.fm/user/followingEvents/1157?access_token=29a055f6fd4a7df45854b38343aa5b1eedb44242

```javascript
{
    "total": 5,
    "offset": 0,
    "limit": 10,
    "data": [
        {
            "id": 8,
            "event": {
                "id": 2658651,
                "title": "Brooklyn Nets vs. New York Knicks",
                "time": "2015-02-06 19:00:00",
                "canceled": 0,
                "url": "http://www.charged.fm/new-york-knicks-tickets/brooklyn-nets-vs-new-york-knicks/02-06-2015/barclays-center/nba/2658651",
                "taxonomy": {
                    "id": 10307,
                    "category": "NBA",
                    "parent": {
                        "id": 103,
                        "category": "Basketball",
                        "parent": {
                            "id": 1,
                            "category": "Sports",
                            "parent": null
                        }
                    }
                },
                "performers": [
                    {
                        "id": 312,
                        "name": "New York Knicks",
                        "url": "http://www.charged.fm/new-york-knicks-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_5407b6c15d1ba.jpg",
                            "medium": "http://media.charged.fm/photos/file_5407b6c33739c.jpg",
                            "large": "http://media.charged.fm/photos/file_5407b6c1eb155.jpg"
                        },
                        "taxonomy": {
                            "id": "10307",
                            "category": "NBA",
                            "parent": {
                                "id": "103",
                                "category": "Basketball",
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
                        }
                    },
                    {
                        "id": 307,
                        "name": "Brooklyn Nets",
                        "url": "http://www.charged.fm/brooklyn-nets-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_540f5e157b440.jpg",
                            "medium": "http://media.charged.fm/photos/file_540f5e1666cce.jpg",
                            "large": "http://media.charged.fm/photos/file_540f5e15a6c6b.jpg"
                        },
                        "taxonomy": {
                            "id": "10307",
                            "category": "NBA",
                            "parent": {
                                "id": "103",
                                "category": "Basketball",
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
                        }
                    }
                ],
                "venue": {
                    "id": 20182,
                    "name": "Barclays Center",
                    "url": "http://www.charged.fm/venue/item/20182/barclays-center",
                    "address": {
                        "address_line1": "Atlantic Avenue",
                        "address_line2": "",
                        "city": "Brooklyn",
                        "state": "New York",
                        "zipcode": "11217",
                        "country": "United States of America"
                    },
                    "location": {
                        "lat": 40.684193673387,
                        "lng": -73.9774425
                    }
                },
                "popularity": 3721,
                "counts": {
                    "followers": 0,
                    "broadcasts": 0
                },
                "tickets": {
                    "price_lowest": 21,
                    "price_highest": 7200,
                    "quantity": 1311
                },
                "type": "event",
                "isfollowing": true
            },
            "time": "2014-12-22T19:10:52-05:00"
        },
        {
            "id": 7,
            "event": {
                "id": 1954,
                "title": "The Grinch Who Stole Christmas",
                "time": "2014-12-26T20:00:00-05:00",
                "images": {
                    "small": "http://media.charged.fm/photos/performer/local/thumb.jpg",
                    "medium": "http://media.charged.fm/photos/performer/local/single.jpg",
                    "large": "http://media.charged.fm/photos/performer/local/single.jpg"
                },
                "url": "http://www.charged.fm/userevent/item/1954/the-grinch-who-stole-christmas",
                "performer": "",
                "venue": {
                    "name": "The Buell Theatre",
                    "address": {
                        "address_line1": "1031 13th St. ",
                        "address_line2": "",
                        "city": "Denver",
                        "state": "Colorado",
                        "country": "United States",
                        "zipcode": "80204"
                    },
                    "location": {
                        "lat": "",
                        "lng": ""
                    }
                },
                "type": "userevent",
                "isfollowing": true
            },
            "time": "2014-12-09T21:41:24-05:00"
        },
        {
            "id": 6,
            "event": {
                "id": 2699872,
                "title": "San Diego Torero at San Diego State Aztecs Basketball",
                "time": "2014-12-04 20:00:00",
                "canceled": 0,
                "url": "http://www.charged.fm/san-diego-toreros-basketball-tickets/san-diego-torero-at-san-diego-state-aztecs-basketball/12-04-2014/viejas-arena/ncaa-baseball/2699872",
                "taxonomy": {
                    "id": 10201,
                    "category": "NCAA Baseball ",
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
                "performers": [
                    {
                        "id": 46094,
                        "name": "San Diego Toreros Basketball",
                        "url": "http://www.charged.fm/san-diego-toreros-basketball-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_54386f0ac26c4.jpg",
                            "medium": "http://media.charged.fm/photos/file_54386f0ca52a8.jpg",
                            "large": "http://media.charged.fm/photos/file_54386f0b8b0c2.jpg"
                        },
                        "taxonomy": {
                            "id": "10301",
                            "category": "NCAA Basketball ",
                            "parent": {
                                "id": "103",
                                "category": "Basketball",
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
                        }
                    },
                    {
                        "id": 46985,
                        "name": "San Diego State Aztecs Basketball",
                        "url": "http://www.charged.fm/san-diego-state-aztecs-basketball-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_543715f964e7a.jpg",
                            "medium": "http://media.charged.fm/photos/file_543715fa27b75.jpg",
                            "large": "http://media.charged.fm/photos/file_543715f984091.jpg"
                        },
                        "taxonomy": {
                            "id": "10301",
                            "category": "NCAA Basketball ",
                            "parent": {
                                "id": "103",
                                "category": "Basketball",
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
                        }
                    }
                ],
                "venue": {
                    "id": 23860,
                    "name": "Viejas Arena",
                    "url": "http://www.charged.fm/venue/item/23860/viejas-arena",
                    "address": {
                        "address_line1": "5500 Canyon Crest Drive",
                        "address_line2": "SDSU",
                        "city": "San Diego",
                        "state": "California",
                        "zipcode": "92115",
                        "country": "United States of America"
                    },
                    "location": {
                        "lat": 32.7789676,
                        "lng": -117.0732307
                    }
                },
                "popularity": 0,
                "counts": {
                    "followers": 0,
                    "broadcasts": 0
                },
                "tickets": {
                    "price_lowest": 0,
                    "price_highest": 0,
                    "quantity": 0
                },
                "type": "event",
                "isfollowing": true
            },
            "time": "2014-12-02T14:41:17-05:00"
        },
        {
            "id": 1,
            "event": {
                "id": 2529788,
                "title": "New England Patriots vs. Buffalo Bills",
                "time": "2014-12-28 13:00:00",
                "canceled": 0,
                "url": "http://www.charged.fm/new-england-patriots-tickets/new-england-patriots-vs-buffalo-bills/12-28-2014/gillette-stadium/nfl/2529788",
                "taxonomy": {
                    "id": 10804,
                    "category": "NFL",
                    "parent": {
                        "id": 108,
                        "category": "Football",
                        "parent": {
                            "id": 1,
                            "category": "Sports",
                            "parent": null
                        }
                    }
                },
                "performers": [
                    {
                        "id": 14743,
                        "name": "New England Patriots",
                        "url": "http://www.charged.fm/new-england-patriots-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_5453a374d472c.jpg",
                            "medium": "http://media.charged.fm/photos/file_5453a375a506b.jpg",
                            "large": "http://media.charged.fm/photos/file_5453a37509039.jpg"
                        },
                        "taxonomy": {
                            "id": "10804",
                            "category": "NFL",
                            "parent": {
                                "id": "108",
                                "category": "Football",
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
                        }
                    },
                    {
                        "id": 50199,
                        "name": "Buffalo Bills",
                        "url": "http://www.charged.fm/buffalo-bills-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_5452b3280f333.jpg",
                            "medium": "http://media.charged.fm/photos/file_5452b328e5a0a.jpg",
                            "large": "http://media.charged.fm/photos/file_5452b3283c0fa.jpg"
                        },
                        "taxonomy": {
                            "id": "10804",
                            "category": "NFL",
                            "parent": {
                                "id": "108",
                                "category": "Football",
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
                        }
                    }
                ],
                "venue": {
                    "id": 4455,
                    "name": "Gillette Stadium",
                    "url": "http://www.charged.fm/venue/item/4455/gillette-stadium",
                    "address": {
                        "address_line1": "1 Patriot Place",
                        "address_line2": "",
                        "city": "Foxborough",
                        "state": "Massachusetts",
                        "zipcode": "02035",
                        "country": "United States of America"
                    },
                    "location": {
                        "lat": 42.0913,
                        "lng": -71.2645
                    }
                },
                "popularity": 25751,
                "counts": {
                    "followers": 0,
                    "broadcasts": 0
                },
                "tickets": {
                    "price_lowest": 162,
                    "price_highest": 436,
                    "quantity": 60
                },
                "type": "event",
                "isfollowing": true
            },
            "time": "1969-12-31T19:00:00-05:00"
        },
        {
            "id": 3,
            "event": {
                "id": 2531873,
                "title": "Detroit Lions vs. Tampa Bay Buccaneers",
                "time": "2014-12-07 13:00:00",
                "canceled": 0,
                "url": "http://www.charged.fm/detroit-lions-tickets/detroit-lions-vs-tampa-bay-buccaneers/12-07-2014/ford-field/nfl/2531873",
                "taxonomy": {
                    "id": 10804,
                    "category": "NFL",
                    "parent": {
                        "id": 108,
                        "category": "Football",
                        "parent": {
                            "id": 1,
                            "category": "Sports",
                            "parent": null
                        }
                    }
                },
                "performers": [
                    {
                        "id": 136,
                        "name": "Detroit Lions",
                        "url": "http://www.charged.fm/detroit-lions-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_5452bc820419b.jpg",
                            "medium": "http://media.charged.fm/photos/file_5452bc82aebb2.jpg",
                            "large": "http://media.charged.fm/photos/file_5452bc82249c6.jpg"
                        },
                        "taxonomy": {
                            "id": "10804",
                            "category": "NFL",
                            "parent": {
                                "id": "108",
                                "category": "Football",
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
                        }
                    },
                    {
                        "id": 428,
                        "name": "Tampa Bay Buccaneers",
                        "url": "http://www.charged.fm/tampa-bay-buccaneers-tickets",
                        "images": {
                            "small": "http://media.charged.fm/photos/file_542079c72eb90.jpg",
                            "medium": "http://media.charged.fm/photos/file_542079ca578d0.jpg",
                            "large": "http://media.charged.fm/photos/file_542079c8048bd.jpg"
                        },
                        "taxonomy": {
                            "id": "10804",
                            "category": "NFL",
                            "parent": {
                                "id": "108",
                                "category": "Football",
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
                        }
                    }
                ],
                "venue": {
                    "id": 4084,
                    "name": "Ford Field",
                    "url": "http://www.charged.fm/venue/item/4084/ford-field",
                    "address": {
                        "address_line1": "2000 Brush St",
                        "address_line2": "",
                        "city": "Detroit",
                        "state": "Michigan",
                        "zipcode": "48226",
                        "country": "United States of America"
                    },
                    "location": {
                        "lat": 42.328245,
                        "lng": -83.0495622
                    }
                },
                "popularity": 0,
                "counts": {
                    "followers": 0,
                    "broadcasts": 0
                },
                "tickets": {
                    "price_lowest": 0,
                    "price_highest": 0,
                    "quantity": 0
                },
                "type": "event",
                "isfollowing": true
            },
            "time": "1969-12-31T19:00:00-05:00"
        }
    ]
}
```
