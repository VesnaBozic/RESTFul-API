# RESTFul-API



***API*** - application programming interface

> An API, or application programming interface, is a set of rules that define how applications or devices can connect to and communicate with each other.

> At the most basic level, an API is a mechanism that enables an application or service to access a resource within another application or service. 

> Api allows different applications built in different technologies to communicate

***One application makes request and send it to other and other application gets request and sends response***

> With API we are building interface so that this two pieces of software can communicate

## SERVER AND CLIENT

***Client*** send request

***SERVER*** sends response

The application or service doing the accessing is called the client, and the application or service containing the resource is called the server.

The separation of concerns is the core theme of the Web’s client-server constraints.

The Web is a client-server-based system, in which clients and servers have distinct
parts to play

***JSON*** is usually used for communication, it is standard now

It's a data format

***JavaScript Object Notation*** is language of communication

***Endpoint*** is a place where we are making request

***REST*** - this is means of communication , like in real communication, are we taking on phone, are we texting , are we takling face to face 

It’s not tied to HTTP, but is associated most commonly with it.

The HTTP API is CRUD (Create, Retrieve, Update, and Delete)

•	 GET = “give me some info” (Retrieve)

•	 POST = “here’s some update info” (Update)

•	 PUT = “here’s some new info” (Create)

•	 DELETE = “delete some info” (Delete)

Databases, web sites, and business applications need to exchange data. This is
accomplished by defining standard data formats such as Extensible Markup Language
(XML) or JavaScript Object Notation (JSON), as well as transfer protocols or Web services
such as the Simple Object Access Protocol (SOAP) or the more popular Representational
State Transfer (REST)

A ***REST API (also known as RESTful API)*** is an application programming interface (API or web API) that conforms to the constraints of ***REST 
architectural style*** and allows for interaction with RESTful web services. REST stands for representational state transfer

### Some APIs, such as SOAP or XML-RPC, impose a strict framework on developers. But REST APIs can be developed using virtually any programming language and support a variety of data formats. The only requirement is that they align to the following six REST design principles - also known as architectural constraints:

1. ***Uniform Resource interface***. All API requests for the same resource should look the same, no matter where the request comes from. The REST API should ensure that the same piece of data, such as the name or email address of a user, belongs to only one uniform resource identifier (URI). Resources shouldn’t be too large but should contain every piece of information that the client might need.

2. ***Client-server decoupling***. In REST API design, client and server applications must be completely independent of each other. The only information the client application should know is the URI of the requested resource; it can't interact with the server application in any other ways. Similarly, a server application shouldn't modify the client application other than passing it to the requested data via HTTP.

3. ***Statelessness***. REST APIs are stateless, meaning that each request needs to include all the information necessary for processing it. In other words, REST APIs do not require any server-side sessions. Server applications aren’t allowed to store any data related to a client request.

The stateless constraint dictates that a web server is not required to memorize the
state of its client applications. As a result, each client must include all of the contextual
information that it considers relevant in each interaction with the web server.

Web servers ask clients to manage the complexity of communicating their
application state so that the web server can service a much larger number of clients. This
trade-off is a key contributor to the scalability of the Web’s architectural style.

4. ***Cacheability***. When possible, resources should be cacheable on the client or server side. Server responses also need to contain information about whether caching is allowed for the delivered resource. The goal is to improve performance on the client side, while increasing scalability on the server side.

5. ***Layered system architecture***. In REST APIs, the calls and responses go through different layers. As a rule of thumb, don’t assume that the client and server applications connect directly to each other. There may be a number of different intermediaries in the communication loop. REST APIs need to be designed so that neither the client nor the server can tell whether it communicates with the end application or an intermediary.

6. ***Code on demand (optional)***. REST APIs usually send static resources, but in certain cases, responses can also contain executable code (such as Java applets). In these cases, the code should only run on-demand.


## How REST APIs work

***REST APIs*** communicate via ***HTTP requests*** to perform standard database functions like creating, reading, updating, and deleting records (also known as CRUD) within a resource. For example, a REST API would use a GET request to retrieve a record, a POST request to create one, a PUT request to update a record, and a DELETE request to delete one. All HTTP methods can be used in API calls.

***A well-designed REST API is similar to a website running in a web browser with built-in HTTP functionality.***

The state of a resource at any particular instant, or timestamp, is known as the resource representation. This information can be delivered to a client in virtually any format including JavaScript Object Notation (JSON), HTML, XLT, Python, PHP, or plain text. JSON is popular because it’s readable by both humans and machines—and it is programming language-agnostic.

Request headers and parameters are also important in REST API calls because they include important identifier information such as metadata, authorizations, uniform resource identifiers (URIs), caching, cookies and more. Request headers and response headers, along with conventional HTTP status codes, are used within well-designed REST APIs.


## PROS 

- Follows the philosophy of the Open Web
- Relatively easy to implement and maintain
- Clearly separates client and server implementations
- Communication isn’t controlled by a single entity
- Information can be stored by the client to prevent multiple calls.
- Can return data in multiple formats (JSON, XML etc.)

## CONS 

- Only works on top of the HTTP protocol
- Hard to enforce authorization and security on top of it


## WE USE IT FOR 

- Social media services
- Social networks (Twitter)
- Web chat services
- Mobile services

## SOAP WE USE FOR

- Financial services (PayPal, Saleforce)
- Payment gateways
- Telecommunication services



## Public API-s

When we create an API, we are allowing others to make use of our service or product to create new applications. Pubilic APIs we can use


## Web Architectural Style

There are two ways to define a system :

- One is to start from a blank slate—an empty whiteboard—with no
initial knowledge of the system being built or the use of familiar
components until the needs are satisfied.

- A second approach is to start with the full set of needs for the
system, and constraints are added to individual components
until the forces that influence the system are able to interact in
harmony with each other.

***REST*** follows the second approach. In order to define a REST architecture, a
null-state is initially defined—a system that has no constraints whatsoever and where
component differentiation is nothing but a myth—and constraints are added one by
one.

***Security*** is another aspect which needs to be considered independently as part
of this framework when rolling out RESTful APIs to the end users.


## REST

REST is resource-based architecture. A resource is accessed via a common interface based on the HTTP standard methods. 
REST asks developers to use HTTP methods explicitly and in a way that’s consistent with the protocol definition.
Each resource is identified by a URL. Every resource should support the HTTP common operations,
and REST allows that resource to have different representations, e.g., text, xml, json, etc. The rest client can ask for specific representation via the HTTP protocol.

HTTP natively supports a mechanism based on headers to tell the server about the
content you expect and you’re able to handle. Based on these hints, the server is
responsible for returning the corresponding content in the correct format.

If the server doesn’t support the requested format, it will send back a 406 status code
(Not Acceptable) to notify the client that made the request.









