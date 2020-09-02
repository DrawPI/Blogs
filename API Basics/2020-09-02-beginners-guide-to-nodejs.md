---
title: 'Beginners guide to Nodejs'
date: '2020-02-09'
author: 'Utkarsh Singh'
---

## Starting Simple

Here's what Node really is: a runtime engine for JavaScript.  
What does this mean for developers?  
Initially, JavaScript was launched only for the client-side Web, meaning Websites. So you could run JS only on the browser.  

One day, somebody split open a browser, extracted the 'engine' that ran JavaScript code from the browser and used that code to make their own local engine. They called this: Node.js.

So when you simply ask yourself how would you run your code if Node didn't exist, you REALLY get its importance.

Node has become almost synonymous with JavaScript today. Almost all frameworks are, in a way running on Node and making our lives easier.

## Node and APIs

Many direct uses of Node include building APIs using Express, Hapi, Koa, etc.  
Express is the most famous of them all.

Here, at DrawPI, we use Node & Express to build our APIs and yours too!  

Let us know in the feedback if you would like some new framework to build your APIs.

Anyway, the simplest (not exclusive) frame of defining an endpoint in an API in express is:
```
app.<method>((req, res) => {
    // Extract information from req body, query or params

    // Use that information for CRUD operations
    // OR
    // Perform certain computations
    // OR
    // Use a 3rd party API to receive or update certain information

    // Return a response
    res.send('OK')
})
```

Extracting information from request fields depends on the data coming in from the client-side.
For example, in a POST Request with payload in req.body, you could do something like:

```
const payload = req.body
```

Or if you know what the elements in req.body are, simply write:
```
const { key } = req.body
```

Well, this is all JavaScript, and we could go on and on with better looking or simpler code to use.

This was Node. Yes, it might not be the mammoth article you were expecting probably, but know that Node is very different than the frameworks you work in or the libraries you use. All that is running on top of this amazing environment.

All the best!