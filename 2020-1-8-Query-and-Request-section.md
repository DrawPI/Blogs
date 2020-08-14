Query parameters:

Have you ever come through long statements in URLs with ( ?, &, and
=), when you type something in search engine and wondered what
they are?

They are called URL(Uniform Resource Locators) with query
parameters. Now what are query parameters? Don’t worry Drawpi
will explain it to you. So, query parameters are a set of parameters
that are used as extensions for URLs to define the specific actions of
the data passed. They appear after the question mark(?) in the URL.

For example:http://127.0.0.1:8000/items/?skip=0&limit=10
Here in this URL the query parameters are skip=0 and limit=0. They
are often optional and non unique.
-Keys added in the query are similar to query parameters used
in the APIs. For example, in “https://abc.com?car=bmw” car is a
query parameter.


-It helps to search for entries in specified database schemas for
the values defined when the API is called.


-Click on +Key button to add a key. The key name should be the
same as an attribute in the schema you want to use this query
parameter to search for a value.


-For example, you create a schema abc with attributes atr1 as
int and atr2 as varchar(255). To search entries in abc by atr1,
atr1 should be a key name in the query.


-To remember what this key does you can write notes in the
What’s this all about input field.
Once you have created a project and a DB schema, you can add
query parameters to each endpoint. These query parameters will
help you to work on the condition block for your endpoint.


REQUEST PARAMETERS:
Request parameters are included in the request body and are used
to send and receive data via REST APIs.
-APIs often have a JSON body, this section helps you to create
that in your API.

-Click on +Key button to create a key. Key can be of 2 types:
Object & String

-String type keys should like query have a name similar to an
attribute in the schema to which they will interact. Used to find
& delete in the schema.

-Object type keys can take any name, but while making request
the keys inside this key should have same name as attributes in
the schema to which they will interact. Used to add in schema.

-For example, you create a schema abc with attributes atr1 as
int and atr2 as varchar(255). To search or delete entries in abc
by atr1, atr1 should be a key with type String.

-For example, to add entries in abc, create key with any name
xyz and type Object. But while calling the api the xyz object
should be as follows:
“xyz”: { “atr1” : VALUE, “atr2” : VALUE}.

-So the xyz should contain keys with name same as attributes in a schema they will interact with.

