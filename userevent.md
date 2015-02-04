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



### **userevent/{id}**

Deployed on branch: `dev`

#### **Description**

Read the userevent data 

#### **Method**

GET

#### **Param**

- id
- password: optional

Example:

```javascript
{
    "status": "success",
    "userevent": {
        "id": "1934",
        "userID": "66784",
        "title": "Dinner and a Suit on CHARGED.fm LIVE",
        "description": "<div class=\"uiHeader fbTimelineAboutMeHeader\" style=\"margin: 15px 15px 15px 22px; color: rgb(20, 24, 35); font-family: Helvetica, Arial, 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12px; line-height: 15.3599996566772px; background-image: none; background-attachment: initial; background-size: initial; background-origin: initial; background-clip: initial; background-position: initial; background-repeat: initial;\"><div class=\"clearfix uiHeaderTop\" style=\"zoom: 1;\"></div></div><div><div><div style=\"text-align: justify;\"><div><font color=\"#062134\" ><span style=\"line-height: normal;\">We've got Dinner and a Suit coming to CHARGED.fm LIVE's Brooklyn studio, Monday @ 2PM for a rare acoustic performance that &nbsp;you won't want to miss!</span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\"><br></span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\">Fueled by momentum from their 2012 LP Since Our Departure, the Jersey-born, Nashville-based rock outfit has spent the past two years in motion. &nbsp;There has been non-stop touring, critical praise and global highlights â€“ all building blocks for a band on the rise â€“ that have laid the groundwork for continued exploration.</span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\">&nbsp;</span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\">And so itâ€™s fitting that Dinner And A Suit has released their new EP STAY on October 7, 2014.</span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\">&nbsp;</span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\">Written on the road, STAY is like a beam into the unified soul of this dedicated, four-piece band â€“ comprised of singer Jonathan Capeci, guitarist Joey Beretta, bassist Anthony Genca and drummer Drew Scheuer.&nbsp;</span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\"><br></span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\">So come on over to CHARGED.fm and live LIVE with us and Dinner and a suit!&nbsp;</span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\"><br></span></font></div><div><font color=\"#062134\" face=\"arial\"><span style=\"line-height: normal;\">Please RSVP to this event to attend!</span></font></div></div></div><div><br></div></div>",
        "startDate": "2014-11-24 00:00:00",
        "endDate": "2014-11-24 00:00:00",
        "venue": {
            "name": "CHARGED.fm Studios",
            "address": {
                "address": null,
                "city": "Brooklyn",
                "state": "New York",
                "zipcode": "11201",
                "country": "United States"
            },
            "coordinates": {
                "latitude": "",
                "longitude": ""
            }
        },
        "tags": "Music-Performance",
        "category": "3",
        "subcategory": "10",
        "public": "yes",
        "url": "http://www.charged.fm/userevent/item/1934",
        "created": "0000-00-00 00:00:00",
        "published": "0000-00-00 00:00:00",
        "updated": "2014-11-14 18:52:18"
    },
    "code": 200
}
```
