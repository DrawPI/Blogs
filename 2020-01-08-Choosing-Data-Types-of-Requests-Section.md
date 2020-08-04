---
title: 'Choosing Data Types of  Requests Section'
date: '2020-01-08'
author: 'Vindhya Srivastava'
---

# Choosing Data Types of Requests Section

DrawPI is on it&#39;s way to bring revulsion in the world of APIs and Backend. All the continuous efforts in bringing the Idea of creating backends without coding in frame optimising is in place.

This website will allow the user to build API(Application program Interface) in the earliest way possible so that their softwares component can learn easily how to interact with the server by sending data to the server.

The ones who are working on projects, models, aspiring to perform front-end development or planning to do something like this that certainly involves APIs to deal with the data management will find this as an amazing platform .

![Imgur](https://i.imgur.com/VqQiZp2.png)

## This blog will pave your way to create APIs in minutes !!

It has been already highlighted in the previous blogs that [DrawPI](https://drawpi.com/) supports int and varchar datatypes with max 255 char for now,but will come up with more featured user interfaces soon.

So I hope that the title of the blog itself invites your attention to know more about the methods of choosing Data Types.

You must be having very basic yet valid questions to ask like &quot; What does the request block actually do to your way of building APIs in DrawPI???&quot; &quot;What if it is ignored???&quot;

So we are here to evidently answer all the queries in the best possible way.

APIs often support JSON bodies to exchange data between script and pages with servers on the web. When you move to the details column you will find a section named as &#39;Request&#39;. You need to add a function in this Conditional block to proceed further and without adding Object(remember it is case sensitive)Key in the Request block you won&#39;t be able to access the next blocks.

Now here it is important to note that there are two keys (_object key and string key_ ) offered while adding a function in DrawPI. Now it&#39;s always a blithe to have two options for one task, but definitely one works the best and other as rest. Here , DrawPI particularly suggests choosing an Object key with any of your desired names to add key.

![Imgur](https://i.imgur.com/VFgGT2s.png)
String key helps to find , replace and delete data in your module.

Object keys can take any name , but while making requests the keys inside this key should have the same name as attributes in the schema to which they will interact.

Now unquestionably, examples clears the cloudy thoughts. So, to advocate the above stated concept of object key, here is an example for your reference .

### Suppose!

To add entries in abc, create a key with any name xyz and type Object. But while calling the api the xyz object should be as follows:
