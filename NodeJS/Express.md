# Express

Express.js, or simply Express, is a free, open-source, lightweight, and fast backend web application framework for Node.js. It is released as open-source software under the MIT License.

It is designed for building single-page, multi-page, and hybrid web applications and APIs. It is called the de facto standard server framework for Node.js. It was founded and developed by TJ Holowaychuk in 2010 and written in JavaScript.

## Q. Features of Express?
* js can be used to design single-page, multi-page, and hybrid web applications and APIs.

* It allows to set up middleware to respond to HTTP/RESTful Requests.

* It defines a routing table to perform different HTTP operations (method and URL).

* It allows to dynamically rendering HTML Pages based on passing arguments to templates.
* It provides high performance because of its ultra-fast I/O. It prepares a thin layer; therefore, the performance is adequate.
* Its MVC-like structure makes it organize the web application into MVC architecture.
* It provides good database support. It supports RDBMS as well as NoSQL databases.
* It is asynchronous and single-threaded.
* Its robust API makes routing easy.

## Is Express.js front-end or backend framework and Why do we use Express.js?
* Express.js or Express is a JavaScript backend framework

* Express.js is an automatically prebuilt Node.js framework that facilitates us to create server-side web applications faster and smarter. The main reason for choosing Express is its simplicity, minimalism, flexibility, and scalability characteristics.

## Q. Write the code to start serving static files in Express.js.

```javascript
app.use(express.static('public'))  
app.use('/static', express.static(path.join(__dirname, 'public')))  
```

## Q. Type of Middleware.
* Application-level Middleware:- The application-level middleware method is used to bind to the app object using app.use() method.

* Router-level Middleware:- The router-level Middleware is used to bind to a specific instance of express.Router().Built-in Middleware: The built-in Middleware was introduced with version 4.x. It ends the dependency on Connect.

* Error-handling Middleware
* Built-in Middleware
* Third-party Middleware
    * Body-parser
    * Cors
    * Mongoose