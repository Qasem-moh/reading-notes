# APIs

* What does REST stand for?

        REST is an architectural style for building distributed systems based on hypermedia REST is independent of any underlying protocol and is not necessarily tied to HTTP.


* REST APIs are designed around a ____.

        Roy Fielding


* What is an identifer of a resource? Give an example.

        https://adventure-works.com/orders/1


* What are the most common HTTP verbs?

        1- REST APIs are designed around resources, which are any kind
         of object, data, or service that can be accessed by the 
         client.

        2- A resource has an identifier, which is a URI that uniquely
           identifies that resource. For example, the URI for a 
           particular customer order might be:
           https://adventure-works.com/orders/1

        3- Clients interact with a service by exchanging 
           representations of resources. Many web APIs use JSON as the 
           exchange format. For example, a GET request to the URI 
           listed above might return this response body:
           {"orderId":1,"orderValue":99.90,"productId":1,"quantity":1}

        4- REST APIs use a uniform interface, which helps to   
           decouple the client and service implementations. For REST
           APIs built on HTTP, the uniform interface includes using 
           standard HTTP verbs to perform operations on resources. 
           The most common operations are GET, POST, PUT, PATCH, and 
           DELETE.

        5-REST APIs use a stateless request model. HTTP requests 
          should be independent and may occur in any order, so keeping 
          transient state information between requests is not
          feasible. 

          The only place where information is stored is in the
          resources 
          themselves, and each request should be an atomic operation. 
          This constraint enables web services to be highly scalable, 
          because there is no need to retain any affinity between 
          clients and specific servers. Any server can handle any 
          request from any client. That said, other factors can limit

         scalability. For example, many web services write to a 
         backend data store, which may be hard to scale out. For more
         information about strategies to scale out a data store, see
         Horizontal, vertical, and functional data partitioning.

        6-REST APIs are driven by hypermedia links that are 
          contained in the representation. For example, the following
          shows a JSON representation of an order. It contains links
          to get or update the customer associated with the order.




* What should the URIs be based on?

        1- Level 0: Define one URI, and all operations are POST 
        requests to this URI.
        2- Level 1: Create separate URIs for individual resources.
        3- Level 2: Use HTTP methods to define operations on resources.
        4- Level 3: Use hypermedia (HATEOAS, described below).


* Give an example of a good URI.

        https://adventure-works.com/orders


* What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

            it might not be possible to map every operation implemented by a web API to a specific resourcen, and its not Good.



* What status code does a successful GET request return?

            200



* What status code does an unsuccessful GET request return?

            404


* What status code does a successful POST request return?

        201


* What status code does a successful DELETE request return?

        204

