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

***JSON*** is usually used for communication, it is standard now

***JavaScript Object Notation*** is language of communication

***Endpoint*** is a place where we are making request

***REST*** - this is means of communication , like in real communication, are we taking on phone, are we texting , are we takling face to face 

A ***REST API (also known as RESTful API)*** is an application programming interface (API or web API) that conforms to the constraints of ***REST 
architectural style*** and allows for interaction with RESTful web services. REST stands for representational state transfer

### Some APIs, such as SOAP or XML-RPC, impose a strict framework on developers. But REST APIs can be developed using virtually any programming language and support a variety of data formats. The only requirement is that they align to the following six REST design principles - also known as architectural constraints:

1. ***Uniform interface***. All API requests for the same resource should look the same, no matter where the request comes from. The REST API should ensure that the same piece of data, such as the name or email address of a user, belongs to only one uniform resource identifier (URI). Resources shouldn’t be too large but should contain every piece of information that the client might need.

2. ***Client-server decoupling***. In REST API design, client and server applications must be completely independent of each other. The only information the client application should know is the URI of the requested resource; it can't interact with the server application in any other ways. Similarly, a server application shouldn't modify the client application other than passing it to the requested data via HTTP.

3. ***Statelessness***. REST APIs are stateless, meaning that each request needs to include all the information necessary for processing it. In other words, REST APIs do not require any server-side sessions. Server applications aren’t allowed to store any data related to a client request.

4. ***Cacheability***. When possible, resources should be cacheable on the client or server side. Server responses also need to contain information about whether caching is allowed for the delivered resource. The goal is to improve performance on the client side, while increasing scalability on the server side.

5. ***Layered system architecture***. In REST APIs, the calls and responses go through different layers. As a rule of thumb, don’t assume that the client and server applications connect directly to each other. There may be a number of different intermediaries in the communication loop. REST APIs need to be designed so that neither the client nor the server can tell whether it communicates with the end application or an intermediary.

6. ***Code on demand (optional)***. REST APIs usually send static resources, but in certain cases, responses can also contain executable code (such as Java applets). In these cases, the code should only run on-demand.


## How REST APIs work

***REST APIs*** communicate via ***HTTP requests*** to perform standard database functions like creating, reading, updating, and deleting records (also known as CRUD) within a resource. For example, a REST API would use a GET request to retrieve a record, a POST request to create one, a PUT request to update a record, and a DELETE request to delete one. All HTTP methods can be used in API calls.

***A well-designed REST API is similar to a website running in a web browser with built-in HTTP functionality.***

The state of a resource at any particular instant, or timestamp, is known as the resource representation. This information can be delivered to a client in virtually any format including JavaScript Object Notation (JSON), HTML, XLT, Python, PHP, or plain text. JSON is popular because it’s readable by both humans and machines—and it is programming language-agnostic.

Request headers and parameters are also important in REST API calls because they include important identifier information such as metadata, authorizations, uniform resource identifiers (URIs), caching, cookies and more. Request headers and response headers, along with conventional HTTP status codes, are used within well-designed REST APIs.


