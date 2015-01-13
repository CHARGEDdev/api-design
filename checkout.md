# Checkout URI

Build the checkout URI with the following parameters below. Always post to `https`

### Parameters
* `tid` - ticket id
* `qty` - quantity of tickets (optional, defaults to max)
* `aid` - affiliate id (optional)
* `sid` - session id (optional)

### Example:
https://www.charged.fm/checkout/secure?tid=ex12132&qty=1

---

##### Note:
You may retrieve the `tid` from the `/event/tickets/id` or `/userevent/tickets/id` endpoints.
