### **User/Create**

Deployed on branch: `api`

#### **Description**

Create new user and return a user api key

#### **Method**

POST

#### **Param**

- username
- password

#### **Example Preview**
```
JSON: http://api.charged.fm/user/create/
XML: http://api.charged.fm/user/create/
```
#### **Endpoint**
```
http://api.charged.fm/user/create/
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/user/create/'optional
```
#### **Example Response**
```
{
  "status": "success",
  "API-Key": "foo"
}
```
