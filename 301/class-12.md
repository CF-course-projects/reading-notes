# CRUD 

### Status Codes Based On REST Methods

In your own words, describe what each group of status code represents:

- 100’s = Informational status codes
- 200’s = Success codes; the client request was accpeted
- 300’s = Redirect codes; the the requested resource is no longer available at the expected location
- 400’s = client error codes; invalid request made
- 500’s = server error codes
<br></br>
- What is a status code 202?
  - Request accepted, processing underway
- What is a status code 308?
  - Permanent redirect: tells client to use another URL to access the resource instead of the current URL.
- What code would you use if an update didn’t return data to a client?
  - 204 No Content
- What code would you use if a resource used to exist but no longer does?
  - 410 Gone
- What is the ‘Forbidden’ status code?
  - 403 Forbidden: Client doesn't have necessary permissions to access the resource.

### Build A REST API With Node.js, Express and MongoDB

- Why do we need to pull our MongoDB database string out of our server and put it into our .env?
  - This enables accessing mongoDB when not running from local host as the env var can be changed when deployed.
- What is middleware?
  - Middleware is code that runs when our server gets a request, but before the request hits a route.
- What does app.use(express.json()) do?
  - This lets the server accept json as a body for requests.
- What does the /:id mean in a route?
  - /:id is a request param 
- What is the difference between PUT and PATCH?
  - PUT is a complete update whereas PATCH is a partial update
- How do you make a default value in a schema?
  - For each property in the schema, you can assign an object, and using the keyword property 'default' you can assign a default value to the key 
- What does a 500 error status code mean?
  - a 500 error means an internal server error
- What is the difference between a status 200 and a status 201?
  - 200: Success code, client response accepted.
  - 201: Success code, created something.
