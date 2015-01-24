### **Cart/Promo**

Deployed on branch: `api`

#### **Description**

Apply Promo Code to the cart.

#### **Method**
POST

#### **Parameters**
- hash: cart hash code
- code: promo code

#### **Endpoint**
```
https://api.charged.fm/cart/promo
```
#### **Example Request**
```
code:Walgreens
hash:aa32014f07ddffb46d158df04c399c8f
```
#### **Example Response**
```
{
    "hash": "aa32014f07ddffb46d158df04c399c8f",
    "items": [
        {
            "tid": 580772,
            "usereventid": 149,
            "price": 13.5,
            "fee": 0
        },
        {
            "tid": 580773,
            "usereventid": 149,
            "price": 13.5,
            "fee": 0
        },
        {
            "tid": 580774,
            "usereventid": 149,
            "price": 13.5,
            "fee": 0
        }
    ],
    "quantity": 3,
    "subtotal": 40.5,
    "fees": 0,
    "total": 34.5,
    "discount": 6,
    "promo": "Walgreens"
}
```
