### **user/signup**

Deployed on branch: `dev`

#### **Description**

user sign up endpoint.

`username` will be automactially generated from `firstname` and `lastname`.

For example: "Hello World" will have `username` hellow , hellow1, hellow2 until the username doesnt confict with others'.

#### **Method**

POST

#### **Param**

- email: email address to register
- password: 5 character at least
- password_repeat: 5 character at least
- firstname: first name
- lastname: last name

Example:

Response:
```javascript
{
  "message": "Success",
  "code": 200
}
```
