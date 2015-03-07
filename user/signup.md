### **user/signup**

Deployed on branch: `dev`

#### **Description**

user sign up endpoint.

`username` will be automactially generated from `firstname` and `lastname`.

For example: "John Doe" will have `username` johnd , johnd1, johnd2 until the username doesnt confict with others'.

#### **Method**

POST

#### **Param**

- `email`: email address to register
- `password`: minimum of 5 characters
- `password_repeat`: minimum of 5 characters, must match `password`
- `firstname`: user's first name
- `lastname`: user's last name
- `username`: letters, numbers and '_' only

Example:

Response:
```javascript
{
  "message": "Success",
  "code": 200
}
```
