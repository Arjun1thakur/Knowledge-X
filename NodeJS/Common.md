
# NodeJS
* Node.js is a server-side JavaScript runtime environment that is built on the Google V8 JavaScript engine. It is an open-source, cross-platform runtime environment that allows developers to build scalable and high-performance applications. Node.js uses an event-driven, non-blocking I/O model that makes it highly efficient and suitable for building real-time applications that require low latency and high throughput.

## Q. What Is Node.js Written In?
* Node.js is written in C, C++, and JavaScript.

## Q. Node.js Architecture and How It Works
* Node.js uses the “Single Threaded Event Loop” architecture to handle multiple clients at the same time.

![Node.js Architecture](https://kinsta.com/wp-content/uploads/2021/03/Nodejs-Architecture.png)

    * Node.js maintains a limited thread pool to serve requests.
    * Whenever a request comes, Node.js places it into a queue.
    * Now, the single-threaded “Event loop”—the core component—comes into the picture. This event loop waits for requests indefinitely.
    * When a request comes in, the loop picks it up from the queue and checks whether it requires a blocking input/output (I/O) operation. If not, it processes the request and sends a response.
    * If the request has a blocking operation to perform, the event loop assigns a thread from the internal thread pool to process the request. There are limited internal threads available. This group of auxiliary threads is called the worker group.
    * The event loop tracks blocking requests and places them in the queue once the blocking task is processed. This is how it maintains its non-blocking nature.

## Q. What is Node.js used for?
* Node is centered around fixing the following problems:

        * Accessing File System
        * Access Database for Information
        * Accessing APIs
        * Accessing System Information  
    
* ***Web development:-***  Node.js is often used for building server-side web applications, such as e-commerce websites, social media platforms, and content management systems. It can be used with popular web frameworks like Express.js and Hapi.js.

* ***Real-time applications:-*** Node.js is particularly suited for building real-time applications like chat applications, gaming platforms, and collaboration tools that require instant updates.

* ***Microservices:-*** Node.js can be used for building microservices, which are small, independent services that work together to form a larger application.

* ***Command-line tools:-*** Node.js can be used for building command-line tools that automate repetitive tasks or streamline workflows.

* ***Internet of Things (IoT):*** Node.js can be used for building IoT applications, as it provides an easy way to interface with hardware and communicate with devices over the network.

* ***APIs:-*** Node.js can be used for building APIs that allow other applications to access data and functionality from your application.

* ***Machine learning:-*** Node.js can be used in machine learning applications, particularly for building web-based machine learning applications.

## Q. Features Of Node.js
* ***Easy—*** Node.js is quite easy to start with. It’s a go-to choice for web development beginners. With a lot of tutorials and a large community—getting started is very easy.
* ***Scalable—*** It provides vast scalability for applications. Node.js, being single-threaded, is capable of handling a huge number of simultaneous connections with high throughput.
* ***Speed—*** Non-blocking thread execution makes Node.js even faster and more efficient.
* ***Packages—*** A vast set of open-source Node.js packages is available that can simplify your work. There are more than one million packages in the NPM ecosystem today.
* ***Strong backend—*** Node.js is written in C and C++, which makes it speedy and adds features like networking support.
* ***Multi-platform—***  Cross-platform support allows you to create SaaS websites, desktop apps, and even mobile apps, all using Node.js.
* ***Maintainable—*** Node.js is an easy choice for developers since both the frontend and backend can be managed with JavaScript as a single language.

## Q. Applications Of Node.js
### Users:- 
    * Twitter
    * Spotify
    * eBay
    * Reddit
    * LinkedIn
    * Godaddy
![Applications Of Node.js](https://kinsta.com/wp-content/uploads/2021/03/nodejs-applications.png)

## Q. Is Node.js Frontend Or Backend?
* A common misconception among developers is that Node.js is a backend framework and is only used for building servers. This isn’t true: Node.js can be used both on the frontend and the backend.

## Q. What Is NPM?
* NPM (short for Node Package Manager) is a software package manager for the JavaScript programming language. It is the default package manager for Node.js, a popular runtime environment that allows developers to run JavaScript on the server-side.

* With NPM, developers can easily install, update, and manage packages (i.e., code modules) that are available from a centralized registry. The registry contains millions of packages that can be used to extend the functionality of Node.js applications, as well as front-end web applications built using tools such as React, Angular, and Vue.js.

* In addition to managing packages, NPM also provides tools for developers to create, publish, and distribute their own packages to the registry. This makes it easy for developers to share their code with others and collaborate on open-source projects.

## Q. What Is CLI?
* CLI stands for Command-Line Interface. It is a type of user interface that allows users to interact with a computer program or system by typing commands into a terminal or command-line interpreter.

* Many operating systems and programming languages provide built-in command-line interfaces, which developers can use to interact with their systems or execute commands. CLI tools are popular among developers and system administrators because they can be automated, scripted, and used to perform tasks quickly and efficiently.

## Q. require --> import

```javascript
    //  import feature in old version 
    let http = require('http')
    // ES6 import
    import http from 'http'
    // but give error because ES6 is in trial Mode.
```
then what we do ...
```json
    //add package.json in same folder and write
    
    {
    "type": "module"
    }
```

## Q. What is Buffer Data?
* In Node Js, buffers are used to store raw binary data. A buffer represents a chunk of memory that is allocated on our computer. The size of the buffer, once set, cannot be changed. A buffer is used to store bytes.

### Buffer Module
* ***The buffers module provides a way of handling streams of binary data.***
```javascript
//  example 
<Buffer 81 2e 71 3b 65 2e 31 2f 61 2e> 
```

## Q. What a byte?
* A byte is a sequence of eight bits. Bits are a basic storage unit for your computer; these bits are used to a  value that can be either 0 or 1. 

## Q. What is dotenv?
* The dotenv package is a great way to keep passwords, API keys, and other sensitive data out of your code. It allows you to create environment variables in a . env file instead of putting them in your code.

## Q. what is REPL?
* REPL stands for Read-Evaluate-Print-Loop, and it's a great way to explore the Node.js features in a quick way.

* The term “REPL” is an acronym for Read, Evaluate, Print and Loop.

    * Read the user input.
    * Evaluate your code (to work out what you mean).
    * Print any results (so you can see the computer’s response).
    * Loop back to step 1 (to continue the conversation).

## Q. What is node module?
* Modules provide a way to re-use code in your Node application.
                
or

* In Node.js, Modules are the blocks of encapsulated code that communicates with an external application on the basis of their related functionality. Modules can be a single file or a collection of multiples files/folders. The reason programmers are heavily reliant on modules is because of their re-usability as well as the ability to break down a complex piece of code into manageable chunks.

### ```Modules are of three types:```
* Core Modules:- Node.js has many built-in modules that are part of the platform and comes with Node.js installation. These modules can be loaded into the program by using the require function.
```javascript
// Example
http:- 	creates an HTTP server in Node.js.
fs:-  used to handle file system.
path:-	includes methods to deal with file paths.
os:- provides information about the operating system.

```

* local Modules:- local modules are created locally in your Node.js application.

```javascript
exports.add = function (x, y) {
	return x + y;
};
	
exports.sub = function (x, y) {
	return x - y;
};
	
exports.mult = function (x, y) {
	return x * y;
};
	
exports.div = function (x, y) {
	return x / y;
};

```
* Third-party Modules:- Third-party modules are modules that are available online using the Node Package Manager(NPM). These modules can be installed in the project folder or globally.
```javascript
// Example
* express
* mongoose
* socket.io
* body-parser
```

## Q. Export?
* The export declaration is used to export values from a JavaScript module.
* Every module can have two different types of export, named export and default export. You can have multiple named exports per module but only one default export.

### ```Named exports:```
```javascript
// export features declared elsewhere
export { myFunction2, myVariable2 };

// export individual features (can export var, let,
// const, function, class)
export let myVariable = Math.sqrt(2);
export function myFunction() {
  // …
}
```

### ```Default exports:``` 

```javascript
// export feature declared elsewhere as default
export { myFunction as default };
// This is equivalent to:
export default myFunction;

// export individual features as default
export default function () { /* … */ }
export default class { /* … */ }
```

## Q. Explain the concept of middleware.
* Middleware is a function that acts as a bridge between two components in the server-side application stack: the server and the application logic. Middleware functions can intercept and manipulate incoming HTTP requests and outgoing HTTP responses, performing tasks such as authentication, logging, error handling, and data processing.

## Q. Explain CORS.
* CORS (Cross-Origin Resource Sharing) is a security mechanism implemented in web browsers that restricts web pages from making requests to a different domain than the one that served the page.
* However, there are cases where it is necessary to make cross-origin requests, such as when an API is hosted on a different domain than the one serving the web page. CORS provides a mechanism for selectively relaxing the Same-Origin Policy and allowing cross-origin requests from specific domains.

## Q. What are JWT tokens?
* JWT stands for JSON Web Token, which is a standard for securely transmitting information as a JSON object between parties. JWTs are often used for authentication and authorization in web applications.

* A JWT token consists of three parts separated by dots (.):
    * Header: Contains information about the type of token and the algorithm used to sign the token.
    * Payload: Contains the actual data being transmitted, such as user ID or other metadata.
    * Signature: Used to verify that the token is authentic and has not been tampered with.

## Q. What is body-parser?
* body-parser is a middleware for Node.js web applications that parses incoming request bodies in a middleware before handlers. It allows the application to easily access the data sent in the body of an HTTP request.

* When a client sends a request to a Node.js server, the request body may contain data in the form of JSON, text, or URL-encoded data. body-parser middleware extracts this data and makes it available to the application in a format that can be easily used.

* There are several different parsers available in body-parser, including:
    * JSON parser: Parses JSON-encoded data and makes it available in the request.body object.
    * URL-encoded parser: Parses URL-encoded data (e.g., form data) and makes it available in the request.body object.
    * Text parser: Parses text data and makes it available in the request.body object.
    * Raw parser: Parses raw data and makes it available in the request.body object.