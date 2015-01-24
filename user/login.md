### **User/Login**

Deployed on branch: `api`

#### **Description**

login user and return a user api key

#### **Method**

POST

#### **Param**

- username: Required. Unique letter and number combination of 1 user.
- password: Required.

#### **Example Preview**
```
JSON: http://api.charged.fm/user/login/
XML: http://api.charged.fm/user/login/optional
```
#### **Endpoint**
```
http://api.charged.fm/user/login/
```
#### **Example Request**
```
$ curl 'http://api.charged.fm/user/login/'
```
#### **Example Response**
```
{
  status: "success",
  API-Key: "foo"
}
```
