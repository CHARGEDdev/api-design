### **Performer/Taxonomy**

Deployed on branch: `api`

#### **Description**

Get a list of a performer by category

#### **Method**
GET

#### **Parameters**
- offset: Optional. Default 0. Offset of Performer listing.
- limit: Optional. Default 10. Limit the num of listed Performers.

#### **Example Preview**
```
JSON: http://api.charged.fm/performer/taxonomy/cid/7
XML: http://api.charged.fm/performer/taxonomy/cid/7.xml
```
#### **Endpoint**
```
http://api.charged.fm/performer/taxonomy/cid/{CategoryID}
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/performer/taxonomy/cid/7?offset=0&limit=3'
```        
#### **Example Response**
```
{
  total: 1019,
  offset: 0,
  limit: 3,
  taxonomy: {
    id: "7",
    category: "Basketball",
    parent: {
      id: "1",
      category: "Sports",
      parent: null
    }
  },
  data: [
    {
      id: 32,
      name: "Atlanta Hawks",
      url: "http://www.charged.fm/performer/item/32/atlanta-hawks",
      images: {
        small: "http://media.charged.fm/photos/file_4e5fcd2593564.jpg",
        medium: "http://media.charged.fm/photos/file_4e5fcd25b6fb4.jpg",
        large: "http://media.charged.fm/photos/file_4e5fcd259dd5f.jpg"
      },
      taxonomy: {
        id: "8",
        category: "NBA",
        parent: {
          id: "7",
          category: "Basketball",
          parent: {
            id: "1",
            category: "Sports",
            parent: null
          }
        }
      }
    },
    {
      id: 66,
      name: "Boston Celtics",
      url: "http://www.charged.fm/performer/item/66/boston-celtics",
      images: {
        small: "http://media.charged.fm/photos/file_4c337f876dfe2.jpg",
        medium: "http://media.charged.fm/photos/file_4c337f8785302.jpg",
        large: "http://media.charged.fm/photos/file_4c337f87a1ff0.jpg"
      },
      taxonomy: {
        id: "8",
        category: "NBA",
        parent: {
          id: "7",
          category: "Basketball",
          parent: {
            id: "1",
            category: "Sports",
            parent: null
          }
        }
      }
    },
    {
      id: 96,
      name: "Chicago Bulls",
      url: "http://www.charged.fm/performer/item/96/chicago-bulls",
      images: {
        small: "http://media.charged.fm/photos/file_4eef725319da3.jpg",
        medium: "http://media.charged.fm/photos/file_4eef725330502.jpg",
        large: "http://media.charged.fm/photos/file_4eef72531efa9.jpg"
      },
      taxonomy: {
        id: "8",
        category: "NBA",
        parent: {
          id: "7",
          category: "Basketball",
          parent: {
            id: "1",
            category: "Sports",
            parent: null
          }
        }
      }
    }
  ]
}
```
