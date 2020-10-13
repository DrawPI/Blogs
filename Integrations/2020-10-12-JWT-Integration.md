---
title: 'How to integrate JWT in your project API'
date: '2020-10-12'
author: 'Utkarsh Singh'
---

Integrating JWT into your project API is really a 2-click process.

- Simply click on Integrations > JWT Authentication. DrawPI will take care of all the things needed to setup and build middlewares. Some new routes for signup(/jwt/signup) and login(/jwt/login) will be created. The documentation of your project API will list these endpoints too to guide you and other developers how to authenticate using your API. To know more about what is actually happening in your code, you can refer this [blog](link).
- When you need to make a route private, you can simply click on Add Middleware > JWT Auth. That's it. Now this route is private and it will require a correct Bearer token in the Authorizations header to authenticate the request.

### How to get the Bearer token to use your API?
The **login** route. The `/jwt/login` route is a POST request that is created in your project API as soon as you add the JWT Integration. It accepts user credentials in the Authorization header as username, password. 
On receiving the correct credentials, it will return a user object and the access token.

All the above information will systematically be presented in the documentation page for your project too.

### How do I save the user?
The **signup** route The `/jwt/signup` route is a POST request that is created in your project API as soon as you add the JWT Integration. It accepts a JSON body with the fields **email**, **password**, **confirm_password** to add the new user to the users table of this project.

The users table must be created with the fields __email__ and __password__ in it.
