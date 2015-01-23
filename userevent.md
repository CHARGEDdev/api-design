### **userevent**

Deployed on branch: `api` `dev`

#### **Description**

Create new userevent. Use POST to create a userevent and a usereventid will be returned in the JSON data.
Reuse that ID in future POST and PUT calls to update the user event. All fields are optional when updating.
A "publish" endpoint will be used to publish an event and double check all data to make sure it's legit.

#### **Method**

POST, PUT

#### **Param**

**POST**

- usereventid (leave out if creating an event and it will return a usereventid, include it when updating)
- title: title of event
- description: decription of event
- startTime: start time - timestamp
- endTime: end time - timestamp
- startDate: day event starts
- endDate: day event ends
- venueTBA: boolean
- venueName: venue name - String
- venueAddress: address of venue - String
- city: name of city - String
- state:  name of state - String
- zipcode: integer
- host: host's username
- hostDescription: description of host
- category
- subcategory
- tags: optional
- displayName: string
- public: boolean
- publicAttendeeList: integer
- password: optional

Example:

```javascript
//incomplete currently
```
