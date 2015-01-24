### **event/tickets**

Deployed on branch: `api`

#### **Description**

Get information and list tickets of a event by event's id. Tickets support pagination by offset and limit.

#### **Method**

GET

#### **Param**

**POST**

- offset: Optional. Default 0. Offset of ticket listing.
- limit: Optional. Default 10. Limit the num of listed tickets.

Example Preview
JSON: http://api.charged.fm/event/tickets/id/2342809
XML: http://api.charged.fm/event/tickets/id/2342809.xml

Endpoint
http://api.charged.fm/event/tickets/id/{EVENT_ID}

Example Request
$ curl 'http://api.charged.fm/event/tickets/id/2342809?offset=0&limit=3'
        
Example:

```javascript
{
   id:2342809,
   title:"Brooklyn Nets at Indiana Pacers",
   time:1365807600,
   url:"http://www.charged.fm/event/item/2342809/brooklyn-nets-at-indiana-pacers",
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
         id:5347,
         name:"Indiana Pacers",
         url:"http://www.charged.fm/performer/item/5347/indiana-pacers",
         images:{
            small:"http://media.charged.fm/photos/file_4e5fc9ef3241d.jpg",
            medium:"http://media.charged.fm/photos/file_4e5fc9ef5cbca.jpg",
            large:"http://media.charged.fm/photos/file_4e5fc9ef3f332.jpg"
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
      }
   ],
   venue:{
      id:21591,
      name:"Bankers Life Fieldhouse",
      url:"http://www.charged.fm/venue/item/21591/bankers-life-fieldhouse",
      address:{
         address_line1:"One Conseco Court",
         address_line2:"125 S. Pennsylvania Street",
         city:"Indianapolis",
         state:"Indiana",
         country:"United States of America",
         zipcode:"46204"
      },
      location:{
         lat:"",
         lng:""
      }
   },
   tickets:{
      total:120,
      offset:0,
      limit:3,
      data:[
         {
            id:21217875,
            uri:"http://www.charged.fm/checkout/item?eid=2342809&tid=21217875",
            retail_price:99.75,
            fee:9.98,
            quantity:4,
            eticket:true,
            section:"19",
            row:"35",
            seats:[

            ],
            splits:[
               2,
               4
            ]
         },
         {
            id:21217877,
            uri:"http://www.charged.fm/checkout/item?eid=2342809&tid=21217877",
            retail_price:72.45,
            fee:7.25,
            quantity:6,
            eticket:false,
            section:"221",
            row:"1",
            seats:[

            ],
            splits:[
               1,
               2,
               3,
               4,
               6
            ]
         },
         {
            id:21217879,
            uri:"http://www.charged.fm/checkout/item?eid=2342809&tid=21217879",
            retail_price:56.7,
            fee:5.67,
            quantity:8,
            eticket:true,
            section:"225",
            row:"14",
            seats:[

            ],
            splits:[
               1,
               2,
               3,
               4,
               5,
               6,
               8
            ]
         }
      ]
   }
}
```
