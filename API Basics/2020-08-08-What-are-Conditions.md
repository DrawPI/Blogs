---
title: 'What are Conditions'
date: '2020-08-08'
author: 'Utkarsh Singh'
---

### Condition Block

![Create Screen](https://github.com/DrawPI/Blogs/public/Screenshot%20from%202020-08-08%2017-17-39.png)

The Condition Block is the heart of building APIs in DrawPI.  
You have created a project, collection and a DB Schema. Now, you need to build an endpoint.

The craziest part about every endpoint is building the logic: what should happen at the backend when that request is made? How should the payload data (query, params, request body) be used?

These questions are taken care of in the Condition Block.  
Let's say a particular endpoint is responsible for adding data into the database. 
You have specified a key in the Object block and now you want to use that key object to store data. That's where the **+ Add** condition comes in.  

- **Add Condition** – allows you to add Object in a schema.
  - First input box shows a list of object request & response
  - Second input box shows a list of schemas. 
  - While calling the API, the data of object selected in first input box will be added to the schema selected in second input box.
  - Make sure keys inside the Object Request while calling the API match the attributes in that schema. OR 
  - If you select a response in first input box, then schema from which that response came should be same as the one selected in second input.
- **Find Condition** – allows you to find entries in the specified schema with criteria.
  - First input box shows a list of query & string request.
  - Second input box shows a list of schemas.
  - Key chosen in first input will be the finding criteria in schema chosen in second input.
  - Third input takes in any value. It acts as a variable to store the result of this find condition. It’s called Response**.
  - Make sure selected key in first inputboxexist in the schema selected in second inputbox.
- **Replace Condition** – allows you to replace an Attribute in Response to a Value.
  - First input allows you to choose among responses.
  - Second input allows you to choose an attribute in that response.
  - Third input takes in a value.oValue in third input is set to the attribute in all entries in the response.
- **Update Condition** – allows you to update an AttributeinResponse to a Value by an Operator.
  - First input allows you to choose among responses.
  - Second input allows you to choose an attribute in that response.
  - Third input takes in +, -, / or *.
  - Fourth input takes in aninteger value.oValuesin the selected attribute in all entries in the response will be updated by Operator & Value in fourth input.
- **Delete Condition** – allows you to delete entries in a schema with criteria specified by queryor string requestor response.
  - First input allows you to choose among query, string request and response.
  - Second input allows you to choose a schema.
  - Query & String Request selected should match an attribute name in the selected schema OR
  - Schema from which the Response came should be same as the selected schema.
- **Response Condition** - allows you to respond with values from the API.
  - Single input allows you to choose among schemas and responses which you want to return when the API succeeds. 
