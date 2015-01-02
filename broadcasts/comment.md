### **broadcasts/comment/{$broadcastID}**

Deployed on branch: `api`, `dev`

#### **Description**

Comment on a broadcast image

#### **Method**

POST

#### **Param**

access_token
broadcastID
comment

Example:

http://api.charged.fm/broadcasts/comment/20

```javscript
{
    "status":"success",
    "broadcastID":20,
    "commentID":129,
    "comment":"Nice broadcast dude!",
    "dateCreated":"2015-01-02T16:44:11-05:00"
    "code":200
}
```



### **broadcasts/comment/{$commentID}**

Deployed on branch: `api`, `dev`

#### **Description**

Update a comment on a broadcast image

#### **Method**

PUT

#### **Param**

access_token
commentID
comment

Example:

http://api.charged.fm/broadcasts/comment/20

```javscript
{
    "status":"success",
    "commentID":129,
    "comment":"Nice broadcast dude!",
    "dateCreated":"2015-01-02T16:44:11-05:00",
    "code":200
}
```
