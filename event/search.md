### **event/search**

Deployed on branch: `api` `dev`

#### **Description**

Berif description of endpoint.

#### **Method**

GET

#### **Param**

- q: search terms
- offset: pagination offset
- limit: pagination size limit
- latlng: comma sperated latlng, example: 40.723301,-74.0029883
- radius: default to 5 miles.
- latlng.ne: bounds search northeast, example: 40.7283442,-73.9958967
- latlng.sw: bounds search southwest, example: 40.7189454,-74.0054619
- pid: search for event of a performer
- cid: search for event of a category
- verbose: append &verbose to enable verbose output, no value needed.

Examples:
* http://api.dev.charged.fm/event/search?limit=100&offset=100&q=new%20york%20yankees
* http://api.dev.charged.fm/event/search?latlng=40.7286587,-73.9925526&radius=1&limit=100&offset=100
* http://api.dev.charged.fm/event/search?pid=321
* http://api.dev.charged.fm/event/search?cid=306&verbose
* http://api.dev.charged.fm/event/search?cid=306&latlng=40.7286587,-73.9925526

```javascript

```
