APIs enable us to develop different kinds of web applications having
operations like CRUD(create, retrieve, update, delete).

Here we can discuss different API methods and their use cases.

[Imgur](https://i.imgur.com/h3K7u72.jpg)

GET API :

We can use GET requests to retrieve resource representation or
information only, we cannot modify it in any way. They do not
change the state of the resources and are said to be the safe
methods. GET APIs should be idempotent, which means it should be
able to make multiple identical requests and must also produce the
same result everytime until another API has changed the state of
resource on the server. If the request URLs refers to a data producing
process, the produced data will be returned in the the response and
not the source text of the process, unless it is the output of the
process.

For any GET API, if the resource is found on the server, then it must
return HTTP response code 200(OK). Incase resource is not found
then it must return HTTP response code 404(Not Found), if GET
request itself is not correctly formed then the server will return to
HTTP response code 400(Bad Request).

Example: HTTP GET http://www.appdomain.com /users

POST API :

We can use post APIs to create new subordinate resources. A file is
subordinate to a directory containing it or a row is subordinate to a
database table.

If a resource has been created on the origin server then the response
201 (created). If the action performed by the POST method does not
result in a resource that can be identified by a URL then the HTTP
response code should be 200 (OK) or 204 (No Content).Responses to
this methods are not cacheable. POST is neither safe or idempotent.

Example: HTTP POST http://www.appdomain.com/users

PUT API :

We can use PUT API’s primarily to update existence resource if a new
resource has been created by the PUT API,the origin server must
inform the user agent via the HTTP response code 201 (Created).
If an existing resource is modified then the HTTP response code is
either 200 (OK) or 204 (No Content). Responses to this method are
not cacheable.

The difference between POST APIs and PUT APIs can be observed in
the URLs. POST requests are made on resource collections whereas
PUT requests are made on a single resource.

Example: HTTP PUT http://www.appdomain.com/users/123

DELETE API:

DELETE APIs are used to delete resources identified by the request
URL. If the response includes an entity .An entity describing the
status, then the HTTP response code should be 200 (OK)

If the actions has been queued then it should be 202 (Accepted)
If the actions has been performed but the response does not include
an entity then the HTTP response code should be 204 (No Content)
DELETE operations are idempotent, if you delete a resource then it is
removed from the collection of resources repeatedly calling DELETE
API on the resource will not change the outcome. However calling
DELETE on a resource for a second time will return a 404 (Not Found)
since it was already removed. Responses to this method are not
cacheable.

Example: HTTP DELETE http://www.appdomain.com/users/123
