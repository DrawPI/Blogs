---
title: 'DrawPI - Building API in minutes'
date: '2020-27-07'
author: 'Utkarsh Singh'
---

Build a good design, materialize a great idea, you still need data to play with your product.
Collect as much as data as you want, you still need to send it back to the client in a systematic, secure manner.
What do you call this systematic, secure manner? APIs.

You are most probably aware of the concepts of an API. You're just wondering how can you build an API in 2 minutes when there are literally 1000+ courses over the internet teaching the intricacies of building it through code that takes hours?!

Well, the short answer is: you design, we code. All you have to do is Create, Define, Declare.

1. Create a project.
2. Define a model (a simple database).
3. Declare your endpoints.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/53qtlbz4ydhaiadi47jm.png)
Have a look at the Create page here. This single screen outscores the manual process of code writing for APIs.  The right pane focuses on building each endpoint, while the left defines the properties for the entire API. Let's look at each component of the page in detail.

### Creating a Project
A Project is equivalent to an API. When you create a project:

1. A domain for the API in the form of \<your-username\>-\<projectname\>.drawpi.com is created. This means your API is now hosted before you even began writing code or declared an endpoint.
2. A database for the project is created.
3. A project folder at DrawPI servers is created to add the automatically generated code as you design endpoints.

### Creating a Collection
Collections modularize your API. Nothing affects the functionality of your API through this. This is just to assort endpoints into certain categories so they become easy to manage at the back-end, and easy to understand while developing the front-end.

### Building a Model
Models is an informal term for your Database. At present, DrawPI supports only MySQL databases, so you can only define an SQL schema. (We are expanding and soon will be back with an option to choose MongoDB too, hence the name Models).
When you create a model, it is basically a table in your projects database. You can define all attributes for your model here.
Isn't it high time the world found a way to build databases without going into the dark terminal or a .sql file?

### Creating an Endpoint
Here's the most amazing part. Creation of an endpoint. Now, a disclaimer first. Designing your endpoint may not enable you to design extremely complex enterprise-level APIs, but if you are smart enough, you can use the Condition Block to build endpoints that you need for your projects.
So let's first try to understand what happens in the code of an endpoint.
![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/4ygdfbz2zm4mfpav2d6n.png)

- We define an endpoint.
- Some data is sent along with the request by the client.
- We perform some manipulations in the database, or perform a query.
- Return a relevant data item or part of it.

This is the natural basic flow of an API for most projects.
The data that endpoints require is used from the data attached with the request object coming in. __req.body, req.params, req.query__, you might have heard of these objects if you are a back-end developer, which are used as payload in POST requests, __/<data-here>, /endpoint?key=<data-here>__ respectively.
We need to expect this data in our endpoint code first. That's what we do in the Query and Request Block.

Next up, is the Condition Block. This defines what you shall do with the data. Basically, the code to run after an endpoint request is made by a client is generated based on the structure of the operations in this block. Using this block requires a separate blog post of itself, but let me tell you the basic operations here.
DrawPI currently supports CRUD operations. This means, you can use the Condition Block to perform any Create, Read, Update, or Delete Operations in your database.
All this can be done just by choosing the operation, and choosing the data which needs to be updated.
This is all you do to build an endpoint, the platform writes the code, and deploys it as soon as you click on 'Launch Endpoint', everything within seconds.

Given this process of building an API, how long do you think it would take you to build yours?
2 minutes? 5 minutes? 15 minutes? We don't expect you to spend more time than that on our Create Page anyway.

And that, is how you can build your API in just under 2 minutes!
Head over to drawpi.com to witness the revolution.

### Who is DrawPI for?
Even though DrawPI is a project that could revolutionize back-end development, it is still in development. This means, you could benefit by making APIs if:
- Your project is a simple one with a few DB tables and endpoints.
- You are a front-end developer who wants to see their Android/iOS/Web App project with something more functional than dummy data.
- You want to build a complex back-end, BUT wished that the plain basic setup code and trivial endpoints could write themselves.

I want to stress on the 3rd customer a little here. DrawPI could be used as a customized boilerplate for any bigger project which is too complex for this platform.
Let's say, I need to build a complex Library System that uses heavy security add-ons like authorization headers, session tokens and cookies - features not currently supported by DrawPI. I will need to write code manually for these.
But, I could build models and define basic endpoints like getting info about a student, about a specific book, querying books in a specific category, etc. using DrawPI tools, and export the code to build on manually. Just imagine how much time a back-end developer saves by simply getting the setup done and trivial endpoints built.
