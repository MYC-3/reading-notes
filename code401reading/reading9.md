# WRRC and Java

## HTTP
[Notes taken from this site](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)

General steps taken:

1. Local processing - find hostname of the request

2. resolve an IP - send a DNS request to a DNS server, DNS server can either send back the requested IP or *defer* to another DNS server until the address is found or the server responds with an error.

3. Establish a TCP Connection - Transport Layer Protocol

4. Send an HTTP request - requests are made up of a "request line", a request header, and a body.

5. Tearing Down and Cleaning up - client and server exchange `fin` and `ack` packets that signify the end of the request/response. Client will then start parsing the data and rendering all relevant data.

## HTTP requests in Java
[Notes take from this site](https://www.baeldung.com/java-http-request)

- `HttpUrlConnection` is a built-in Java class that can be used to perform HTTP requests.
- The disadvantage to using `HttpUrlConnection` is that it can be more cumbersome than other HTTP libraries.
- Requests can be created using the `openConnection()` method to create an object which can then make all types of requests; GET, POST, PUT, DELETE, etc.
- `HttpUrlConnection` is capable of adding paramters to requests, setting request headers, configuring timeouts, handling cookies/redirects, and reading the response.

[Back to HOME](../README.md)