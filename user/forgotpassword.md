### **user/forgotpassword/{id}**

Deployed on branch: `api` | `dev`

#### **Description**

this endpoint will reset the password for the account of given email address, and send an email to that account.

#### **Method**

GET

#### **Param**

- `email`: the email address used to register with CHARGED.fm

#### **Response**

```sh
curl http://api.dev.charged.fm/user/forgotpassword?email=haha@gmail.com
```
if success

```javascript
{
    "message": "Success",
    "code": 200
}
```


