# Express REST API

## Name 3 real world use cases where you’d want to change the request with custom middleware

1-Encrypting a password or sensitive information.

2-Using `methodOverride` to utilize `put` and `delete` methods instead of `post`.

3-To process incoming information for statistics and analytics.

---

## True or false: The route handler is middleware?

If the route Handler is the last function in a route (doesn't have or need a next() parameter), then there is no need to call it a middleware... because it is the end point that will send the response.

---

## In what ways can a middleware function end the process and send data to the browser?

By sending a response and not using `next();`... or by passing a parameter in `next()` which will use an error handler.

---

## At what point in the request lifecycle can you “inject” middleware?

Anywhere before reaching the final function (the handler) which is the end point.

---

## What can cause express to error with “Request headers sent twice, cannot start a second response”

This happens when a server tries to send more than one response to the client per one request. [source](https://www.codementor.io/@oparaprosper79/understanding-node-error-err_http_headers_sent-117mpk82z8)
