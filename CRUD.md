# CRUD


### In your own words, describe what each group of status code represents:

* 100’s = informational status codes,  usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client.

* 200’s = These are the success codes. They tell the client that its request was accepted. 

* 300’s = These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. 

* 400’s = These are the client error codes. They are all about invalid requests a client sent to a server.

* 500’s =These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server.

### What is a status code 202?

*  This code tells the client that the request was valid, but its processing will finish sometime in the future.

### What is a status code 308?

* tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

### What code would you use if an update didn’t return data to a client?

* 204 No content

### What code would you use if a resource used to exist but no longer does?

410 gone.

### What is the ‘Forbidden’ status code?

* The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

### Why do we need to pull our MongoDB database string out of our server and put it into our .env?

* to insert our PORT and connect it.

### What is middleware?

* Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system.

### What does app.use(express.json()) do?

* calls json which is a method that is built inside the express, it converts the objects to arrays or strings

### What is the difference beween PUT and PATCH?

* **PUT** requires the client to send an entire representation of a resource to update it.

* **PATCH** requires the client only send parts of the representation of the resource to update it.

### What does a 500 error status code mean?

*  indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.

### What is the difference between a status 200 and a status 201?

* 200 status : the request was received and understood and is being processed. 

* 201 status :  request was successful and as a result, 