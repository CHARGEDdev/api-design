### **event/list**

Deployed on branch: `api`

#### **Description**

List All Event, supported filter by performer, venue and category.

#### **Method**

GET

#### **Param**

**POST**

- offset: Optional. Default 0. Offset of Event listing.
- limit: Optional. Default 10. Limit the num of listed Event.
- pid: Optional. filter on performer's id
- vid: Optional. Filter on venue's id
- cid: Optional. Filter on category's id

Example Preview
JSON: http://api.charged.fm/event/list/
XML: http://api.charged.fm/event/list.xml

Endpoint
http://api.charged.fm/event/list/

Example Request
$ curl 'https://api.charged.fm/event/list?pid=307&vid=20182&cid=1&limit=3'
        
Example:

```javascript
{
   total:15,
   offset:0,
   limit:3,
   data:[
      {
         id:2344189,
         title:"Washington Wizards at Brooklyn Nets",
         time:1366068600,
         url:"http://www.charged.fm/event/item/2344189/washington-wizards-at-brooklyn-nets",
         taxonomy:{
            id:"8",
            category:"NBA",
            parent:{
               id:"7",
               category:"Basketball",
               parent:{
                  id:"1",
                  category:"Sports",
                  parent:null
               }
            }
         },
         performers:[
            {
               id:307,
               name:"Brooklyn Nets",
               url:"http://www.charged.fm/performer/item/307/brooklyn-nets",
               images:{
                  small:"http://media.charged.fm/photos/file_50649189ab8d3.jpg",
                  medium:"http://media.charged.fm/photos/file_50649189c85c1.jpg",
                  large:"http://media.charged.fm/photos/file_50649189b35d6.jpg"
               },
               taxonomy:{
                  id:"8",
                  category:"NBA",
                  parent:{
                     id:"7",
                     category:"Basketball",
                     parent:{
                        id:"1",
                        category:"Sports",
                        parent:null
                     }
                  }
               }
            },
            {
               id:481,
               name:"Washington Wizards",
               url:"http://www.charged.fm/performer/item/481/washington-wizards",
               images:{
                  small:"http://media.charged.fm/photos/file_4c3394d1c740b.jpg",
                  medium:"http://media.charged.fm/photos/file_4c3394d1d9135.jpg",
                  large:"http://media.charged.fm/photos/file_4c3394d1f044f.jpg"
               },
               taxonomy:{
                  id:"8",
                  category:"NBA",
                  parent:{
                     id:"7",
                     category:"Basketball",
                     parent:{
                        id:"1",
                        category:"Sports",
                        parent:null
                     }
                  }
               }
            }
         ],
         venue:{
            id:20182,
            name:"Barclays Center",
            url:"http://www.charged.fm/venue/item/20182/barclays-center",
            address:{
               address_line1:"Atlantic Avenue",
               address_line2:"",
               city:"Brooklyn",
               state:"New York",
               country:"United States of America",
               zipcode:"11217"
            },
            location:{
               lat:"40.681866782543686",
               lng:"-73.97572288844742"
            }
         }
      },
      {
         id:2344289,
         title:"Detroit Pistons at Brooklyn Nets",
         time:1366243200,
         url:"http://www.charged.fm/event/item/2344289/detroit-pistons-at-brooklyn-nets",
         taxonomy:{
            id:"8",
            category:"NBA",
            parent:{
               id:"7",
               category:"Basketball",
               parent:{
                  id:"1",
                  category:"Sports",
                  parent:null
               }
            }
         },
         performers:[
            {
               id:307,
               name:"Brooklyn Nets",
               url:"http://www.charged.fm/performer/item/307/brooklyn-nets",
               images:{
                  small:"http://media.charged.fm/photos/file_50649189ab8d3.jpg",
                  medium:"http://media.charged.fm/photos/file_50649189c85c1.jpg",
                  large:"http://media.charged.fm/photos/file_50649189b35d6.jpg"
               },
               taxonomy:{
                  id:"8",
                  category:"NBA",
                  parent:{
                     id:"7",
                     category:"Basketball",
                     parent:{
                        id:"1",
                        category:"Sports",
                        parent:null
                     }
                  }
               }
            },
            {
               id:137,
               name:"Detroit Pistons",
               url:"http://www.charged.fm/performer/item/137/detroit-pistons",
               images:{
                  small:"http://media.charged.fm/photos/file_510ac24803066.jpg",
                  medium:"http://media.charged.fm/photos/file_510ac2482c48a.jpg",
                  large:"http://media.charged.fm/photos/file_510ac2480ff6e.jpg"
               },
               taxonomy:{
                  id:"8",
                  category:"NBA",
                  parent:{
                     id:"7",
                     category:"Basketball",
                     parent:{
                        id:"1",
                        category:"Sports",
                        parent:null
                     }
                  }
               }
            }
         ],
         venue:{
            id:20182,
            name:"Barclays Center",
            url:"http://www.charged.fm/venue/item/20182/barclays-center",
            address:{
               address_line1:"Atlantic Avenue",
               address_line2:"",
               city:"Brooklyn",
               state:"New York",
               country:"United States of America",
               zipcode:"11217"
            },
            location:{
               lat:"40.681866782543686",
               lng:"-73.97572288844742"
            }
         }
      },
      {
         id:2341651,
         title:"Philadelphia 76ers at Brooklyn Nets",
         time:1365550200,
         url:"http://www.charged.fm/event/item/2341651/philadelphia-76ers-at-brooklyn-nets",
         taxonomy:{
            id:"8",
            category:"NBA",
            parent:{
               id:"7",
               category:"Basketball",
               parent:{
                  id:"1",
                  category:"Sports",
                  parent:null
               }
            }
         },
         performers:[
            {
               id:307,
               name:"Brooklyn Nets",
               url:"http://www.charged.fm/performer/item/307/brooklyn-nets",
               images:{
                  small:"http://media.charged.fm/photos/file_50649189ab8d3.jpg",
                  medium:"http://media.charged.fm/photos/file_50649189c85c1.jpg",
                  large:"http://media.charged.fm/photos/file_50649189b35d6.jpg"
               },
               taxonomy:{
                  id:"8",
                  category:"NBA",
                  parent:{
                     id:"7",
                     category:"Basketball",
                     parent:{
                        id:"1",
                        category:"Sports",
                        parent:null
                     }
                  }
               }
            },
            {
               id:349,
               name:"Philadelphia 76ers",
               url:"http://www.charged.fm/performer/item/349/philadelphia-76ers",
               images:{
                  small:"http://media.charged.fm/photos/file_503e3ecb83f0f.jpg",
                  medium:"http://media.charged.fm/photos/file_503e3ecba5e01.jpg",
                  large:"http://media.charged.fm/photos/file_503e3ecb8db47.jpg"
               },
               taxonomy:{
                  id:"8",
                  category:"NBA",
                  parent:{
                     id:"7",
                     category:"Basketball",
                     parent:{
                        id:"1",
                        category:"Sports",
                        parent:null
                     }
                  }
               }
            }
         ],
         venue:{
            id:20182,
            name:"Barclays Center",
            url:"http://www.charged.fm/venue/item/20182/barclays-center",
            address:{
               address_line1:"Atlantic Avenue",
               address_line2:"",
               city:"Brooklyn",
               state:"New York",
               country:"United States of America",
               zipcode:"11217"
            },
            location:{
               lat:"40.681866782543686",
               lng:"-73.97572288844742"
            }
         }
      }
   ]
}
```
