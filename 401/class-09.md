# OAuth

* **OAuth** is "an open standard for access delegation" ... In other words, OAuth serves as a way to give users the ability to grant application access to services, without giving the application their password. 

* Through a series of "handshakes", an application such as an Express Web Server asks the user if it's ok to login as them at some remote service, and then begins the process of authentication and access.

* Remote service (i.e. Google) contacts the application with a one-time-use Code

* `` user give Application ==> `` **OAuth with specific permissions** ``Application logIN using X==> then give it TOKEN to be able to access the remot servesic as user``

# Access Code
* First the client needs to grant the application permission. To do this you need to provide an <a> tag that will take them to the service's authorization page. <a> tag should pass the following information through a query string to the authorization server. 

* `response_type=code` indicates that your server wants to receive an authorization code
* `client_id=<your client id>` tells the authorization server which app the user is granting access to
* `redirect_uri=<your redirect uri>` tells the auth server which server endpoint to redirect to
* `scope=<list of scopes>` tells the auth server what you want the user to give access to
* `state=<anything you want>` a place where you can store info to pass to your server if you want

### Access Token

If the users grants access to the application, the authorization server will redirect to a provided redirect URI callback with a "code". Once you have this code, you can exchange it for an access token by making a `POST` request to the authorization server and providing the following information:

- `grant_type=authorization_code`
- `code=<the code your received`
- `redirect_uri=REDIRECT_URI` must be same as the redirect URI your client provided
- `client_id=<your client id>` tells the authorization server which application is making the requests
- `client_secret=<your client secret>` authenticates that the application making the request is the application registered with the `client_id`
- Once you get an access token, you can use it to make API calls to the service on behalf of that user