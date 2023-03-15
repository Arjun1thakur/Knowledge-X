# HTTP

## What is HTTP Module?
* Node.js has a built-in module called HTTP, which allows Node.js to transfer data over the Hyper Text Transfer Protocol (HTTP).
* The HTTP module can create an HTTP server that listens to server ports and gives a response back to the client.

```javascript
// Example:-
// import http module
var http = require('http');

//create a server object:
http.createServer(function (req, res){ //write a response to the client
  res.write('Hello World!');
//end the response
  res.end(); 
}).listen(8080); 
//the server object listens on port 8080
```

# What is HTTP Header?
* An HTTP header is a field of an HTTP request or response that passes additional context and metadata about the request or response.

```javascript
// Example:-
var http = require('http');
http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/html'});
  res.write('Hello World!');
  res.end();
}).listen(8080);
```

# What is Routing?
* Routing defines the way in which the client requests are handled by the application endpoints.

```javascript
var http = require('http');

// Create a server object
http.createServer(function (req, res) {	
// http header
	res.writeHead(200, {'Content-Type': 'text/html'});
	var url = req.url;
	if(url ==='/about') {
		res.write(' Welcome to  about us page');
		res.end();
	}
	else if(url ==='/contact') {
		res.write(' Welcome to contact us page');
		res.end();
	}
	else {
		res.write('Hello World!');
		res.end();
	}
}).listen(3000, function() {
	
	// The server object listens on port 3000
	console.log("server start at port 3000");
});

```

## HTTP Methods:-
* ***GET:-*** GET is used to request data from a specified resource.
```javascript
//  Some notes on GET requests:-

* GET requests can be cached
* GET requests remain in the browser history
* GET requests can be bookmarked
* GET requests should never be used when dealing with sensitive data
* GET requests have length restrictions
* GET requests are only used to request data (not modify)
```

* ***POST:-*** POST is used to send data to a server to create/update a resource.
```javascript
// Some notes on POST requests:-

* POST requests are never cached
* POST requests do not remain in the browser history
* POST requests cannot be bookmarked
* POST requests have no restrictions on data length
```
* ***PUT:-***
    * PUT is used to send data to a server to create/update a resource.
    * The difference between POST and PUT is that PUT requests are idempotent. That is, calling the same PUT request multiple times will always produce the same result. In contrast, calling a POST request repeatedly have side effects of creating the same resource multiple times.
* ***HEAD:-***
    * HEAD is almost identical to GET, but without the response body.
    * In other words, if GET /users returns a list of users, then HEAD /users will make the same request but will not return the list of users.
    * HEAD requests are useful for checking what a GET request will return before actually making a GET request - like before downloading a large file or response body.
* ***DELETE:-*** The DELETE method deletes the specified resource.
* ***PATCH:-*** The PATCH method is used to apply partial modifications to a resource.
* ***OPTIONS:-*** The OPTIONS method describes the communication options for the target resource.
* ***CONNECT:-*** The CONNECT method is used to start a two-way communications (a tunnel) with the requested resource.
* ***TRACE:-*** The TRACE method is used to perform a message loop-back test that tests the path for the target resource (useful for debugging purposes).

##	Q. Difference between HTTP and HTTPS
***HTTP (Hypertext Transfer Protocol) and HTTPS (Hypertext Transfer Protocol Secure) are both protocols used for transferring data over the internet, but they differ in their security and encryption mechanisms.***
###	```Some key differences between HTTP and HTTPS:```

* Security: HTTPS is more secure than HTTP because it encrypts data being sent over the internet, which makes it more difficult for attackers to intercept and tamper with the data.
* Encryption: HTTP does not encrypt data being sent over the internet, whereas HTTPS encrypts data using SSL/TLS.
* Port: HTTP typically uses port 80, while HTTPS typically uses port 443.
* Speed: HTTPS can be slightly slower than HTTP because of the additional processing required to encrypt and decrypt data.
* Certificates: HTTPS requires a digital SSL/TLS certificate to establish a secure connection between the client and server, whereas HTTP does not require a certificate.