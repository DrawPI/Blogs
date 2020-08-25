---
title: 'Explanation of Query Section'
date: '2020-01-08'
author: 'Vindhya Srivastava'
---

# Explanation of Query Section

[DrawPI](https://drawpi.com/) aims to provide the best possible way of building API to those enthusiastic formulators who are working under any project or hold the potential to work under such projects where API are needed to organise their data .

![Imgur](https://i.imgur.com/QgYKA5q.png)

Time to have an in-depth knowledge of one parameter featured in APIs. Before that let&#39;s have a look on what API Parameter is all about!!!

## API Parameter

Parameters are known as variable parts of a resource , which means that it identifies what sort of action the user is intended to take on the resource.

The people who want to build API are required to choose the parameter they want for their endpoint.

![Imgur](https://i.imgur.com/QFV0qSj.png)

There are mainly four categories of Parameter , we are here to discuss &#39;Query Parameter &#39; in detail.

### Query Parameter

These parameters are supposed to be the most common parameter that appears at the end of the **URL** after the question mark(?). The string of query parameters appears to contain a question mark, the parameter and the real value.

In nutshell, Query Parameter acts as an extension to your resource locator that will enable you to define the performance of the data being passed.

![Imgur](https://i.imgur.com/u1XG3iJ.png)

Now in DrawPI, the query parameter is defined under the details column .

You will find an option to add key &#39;+key&#39; under the query block which is similar to query parameters used in API as mentioned above. You just need to click on **&#39;+key&#39;** but make sure that the key you add should have a similar name as that of the attribute in the schema .

The screen is displayed below.

![Imgur](https://i.imgur.com/meciPZA.png)

Let&#39;s take an example!

Suppose that you build a schema &#39;Hello&#39; with attribute atr1 as int and atr2 as varchar .To search entries in Hello by atr1, atr1 should be a key name in the query.

This was all about the explanation of the parameters in API and how DrawPI expects it&#39;s user to perform .
