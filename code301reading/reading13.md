# CRUD

[Questions were answered from this site](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

1. In your own words, describe what each group of status code represents:
  - 100’s = Informational
  - 200’s = Success
  - 300’s = Redirection because the location isn't available
  - 400’s = Invalid request (timeout, authentification, etc)
  - 500’s = Server error
2. What is a status code 202?
  - Accepted. Asynchronus valid request.
3. What is a status code 308?
  - Permanent Redirect. 
4. What code would you use if an update didn’t return data to a client?
  - 204
5. What code would you use if a resource used to exist but no longer does?
  - 410
6. What is the ‘Forbidden’ status code?
  - 403

[Questions were answered from this video](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
  - It holds sensitive information that won't be public to whoever accesses the code.
2. What is middleware?
  - code that runs when the server gets a request but before it gets passed to your routes.
3. What does `app.use(express.json())` do?
  - Allows the server to use json as a body.
4. What does the /:id mean in a route?
  - Parameter, you can access by typing `req.params.id`
5. What is the difference beween `PUT` and `PATCH`?
  - `PATCH` will update only what the user inputted.
  - `PUT` will update everything.
6. How do you make a default value in a schema?
  - you can add a `default: ` property in your schema.
7. What does a `500` error status code mean?
  - Internal Server Error.The server encountered an error.
8. What is the difference between a status `200` and a status `201`?
  - `200` = everything was successful. Just a general success.
  - `201` = successfully created an object. More specific.

[Back to HOME](../README.md)