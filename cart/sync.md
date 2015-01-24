### **Cart/Sync**

Deployed on branch: `api`

#### **Description**

create cart, add, delete tickets. every tickets will be on hold for 5mins in the cart.

#### **Method**
PUT

#### **Parameters**
- tickets: an array of tickets encoded in json
- hash: cart hash, if not give new cart will be created

#### **Endpoint**
```
http://api.charged.fm/cart/add/
```
##### **Create Cart Example Request**

http://api.charged.fm/cart/sync/

tickets: {"tickets":[{"tid":580772,"action":"add"},{"tid":580773,"action":"add"},{"tid":580774,"action":"add"}]}
          
#### **Example Response**
```
{
    "hash": "735318980e9d7bf4e0fc15267f0ce38e",
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
    "total": 40.5,
    "sync_success": [
        580772,
        580773,
        580774
    ],
    "sync_failed": []
}
```        
##### **add,delete tickets Example Request**

http://api.charged.fm/cart/sync/
```
tickets:{"tickets":[{"tid":580775,"action":"add"},{"tid":580776,"action":"add"},{"tid":580774,"action":"delete"}]}
hash:735318980e9d7bf4e0fc15267f0ce38e
```        
#### **Example Response**
```
{
    "hash": "735318980e9d7bf4e0fc15267f0ce38e",
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
            "tid": 580775,
            "usereventid": 149,
            "price": 13.5,
            "fee": 0
        },
        {
            "tid": 580776,
            "usereventid": 149,
            "price": 13.5,
            "fee": 0
        }
    ],
    "quantity": 4,
    "subtotal": 54,
    "fees": 0,
    "total": 54,
    "sync_success": [
        580775,
        580776,
        580774
    ],
    "sync_failed": []
```
