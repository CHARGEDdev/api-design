# Checkout URI

Build the checkout URI with the following parameters below. 

Always post to `https`

### Parameters
* `tid`: ticket id (required)
* `qty`: quantity of tickets (optional, defaults to max available)
* `aid`: your affiliate id, to track your referrals (optional)
* `sid`: your session id, to track specific sessions (optional)
* `access_token`: access token of currently logged in user, to auto-login in webview (optional)

**Note**: You may retrieve the `tid` from the `/event/tickets/{id}` or `/userevent/tickets/{id}` endpoints.


### Example:
https://www.charged.fm/checkout/item?tid=ex12132&qty=1
