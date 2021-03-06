### Affiliate Checkout Endpoints

We will use _Andy The Affiliate_'s access token for demonstration purposes. Her details are below. **Be sure to use HTTPS for all requests.**

* `access_token`: b98da03282359144452fe91fd3032da1c0a5f65f  



#### 1. ticket/validate

The response is basically using the same structure with `event/tickets` endpoint but returning the no-cached ticket data with detailed fees and shipping information.
The endpoint is optional since only electronic and real-time tickets are fed to the Affiliate.

**Method:** GET

**Param:**

- `access_token`: your affiliate's access token
- `eid`: event id
- `tid`: ticket id

**Example Request:**

[https://api.charged.fm/ticket/validate?access_token=b98da03282359144452fe91fd3032da1c0a5f65f&eid=2658651&tid=ex1412633](https://api.charged.fm/ticket/validate?access_token=b98da03282359144452fe91fd3032da1c0a5f65f&eid=2658651&tid=ex1412633)

**Example Response:**

```
{
    "id": "ex1412633",
    "eid": 2658651,
    "retail_price": 117,
    "quantity": 8,
    "eticket": true,
    "willcall": false,
    "instant": false,
    "section": "226",
    "row": "16",
    "seats": [],
    "notes": "emailable",
    "splits": [
        1,
        2,
        3,
        4,
        5,
        6,
        8
    ],
    "fees_mapping": {
        "1": 0,
        "2": 0,
        "3": 0,
        "4": 0,
        "5": 0,
        "6": 0,
        "7": 0,
        "8": 0
    },
    "shipping_methods": [
        {
            "name": "eticket",
            "fee": 0
        }
    ]
}
```


---


#### 2. affiliate/checkout

The endpoint will place order on CHARGED.fm’s platform, and return the order information for future reference.

Some of the parameters are optional since the transaction happens on the Affiliate’s side and all tickets are e-ticket. But we still listed all possible parameters to help better understand how our affiliate checkout works.

**Method:** POST

**Param:**

- `access_token`
- `eid`: event id
- `tid`: ticket id
- `qty`: quantity to purchase
- `customer`: customer information in JSON Example: 

```
  {
    "first_name": "Bill",
    "last_name": "McBuyermanamon",
    "email": "test@gmail.com",
    "phone_number": "917-000-0000",
    "address": {
      "first_name": "Billford",
      "last_name": "McBuyermanamon",
      "address_line1": "1 Broadway",
      "address_line2": "Apt PH1",
      "city": "New York",
      "state": "NY",
      "zipcode": "10004",
      "country": "US"
    },
    "billing_address": {
      "first_name": "Bartholomew",
      "last_name": "McBuyermanamon",
      "address_line1": "1 Broadway",
      "address_line2": "Apt PH1",
      "city": "New York",
      "state": "NY",
      "zipcode": "10004",
      "country": "US"
    }
  }
  
```

Since the transaction happens on the affiliate’s side.  
We need **at least** the minimal amount of information to handle customer service and to work with our sellers.
Please provide:

```
  {
    "first_name": "John",
    "last_name": "Dollarshire",
    "email": "john.dollarshire@gmail.com",
    "phone_number": "917-718-0212",
    "address": {
      "first_name": "John",
      "last_name": "Dollarshire",
      "address_line1": "10 Maiden Ln",
      "address_line2": "Apt 30G",
      "city": "New York",
      "state": "NY",
      "zipcode": "10038",
      "country": "US"
    }
  }
```

- shipping: shipping method in JSON 

```
  {
      "name": "eticket",
      "fee": 0
  }
```
	
You can **ignore** this param, since the transaction happens on the affiliate’s side. And all tickets are e-ticket. 

- payment: payment information in JSON 

```
  {
    "amount": 100.00,
    "type": "credit_card",
    "credit_card": {
      "type": "visa",
      "number": "4111111111111111",
      "expire": "0420",
      "cvv": "000"
    }
  }
```

You can **ignore** this param, since the transaction happens on the affiliate’s side. 

**Example Request:**

**This ticket in the example is a test ticket on our site, it's safe to POST the information if you want to test.**

[https://api.charged.fm/affiliate/checkout?access_token=b98da03282359144452fe91fd3032da1c0a5f65f](https://api.charged.fm/affiliate/checkout?access_token=b98da03282359144452fe91fd3032da1c0a5f65f)

```
eid: 2839016
tid: ex12132
qty: 1
customer: {"first_name":"Andy","last_name":"Affiliato","email":"andy@gmail.com","phone_number":"718-212-9170","address":{"first_name":"Andrew","last_name":"Affiliato","address_line1":"10 John St","address_line2":"Apt 1A","city": "New York","state": "NY","zipcode": "10001","country": "US"}}
````

**Example Response:**
```
{
    "code": 200,
    "message": "Success",
    "order": {
        "orderId": "111222",
        "orderNumber": "11412111222"
    }
}
````

Save at least `orderId` for future API requests. `orderNumber` is more for a customer service reference.

**If failed:**
```
{
    "code": 400,
    "message": "a detailed error response"
}
```


---


#### 3. affiliate/orders

**Method:** GET

**Param:**

- `access_token`
- `orderId`: optional: omit if you wish to view all your recent orders by date
- `limit`: defaults to 10

**Example Request:**  
[https://api.charged.fm/affiliate/orders?access_token=b98da03282359144452fe91fd3032da1c0a5f65f&orderId=195207](https://api.charged.fm/affiliate/orders?access_token=b98da03282359144452fe91fd3032da1c0a5f65f&orderId=195207)

**Example Response:**

```
{
    "orderId": 195207,
    "orderNumber": "11509195207",
    "eticket": true,
    "quantity": 1,
    "status": "DELIVERED",
    "ticketFile": "https://web1.charged.fm/orders/tickets/11509195207/0a507aa920a8bfd2f43c9ac1440f9ad6.pdf"
}
```

The status in the response may have the following values:

- **PENDING**: the order just placed.
- **ACCEPTED**: the order has been accepted, waiting for ticket uploading.
- **REJECTED**: the order is rejected, you may need to refund your customer.
- **DELIVERED**: the order’s ticket has been uploaded. There will be an extra field **ticketFile** for you to download the ticket file.


---

#### Please note: 

1) You may need to check this endpoint regularly after the order is placed to deliver tickets to your customers promptly.

2) After you have integrated these endpoints, you may request test tickets data to begin testing.

3) If there are any questions or further information you think is necessary to add to the endpoints, please let us know.
