---
title: 'How to manage your Database'
date: '2020-20-08'
author: 'Utkarsh Singh'
---

## Database Schema

Managing databases is a new feature on the DrawPI platform for the August release.  
  
Simply creating a Database schema for your API is not enough. Being a developer is about having complete control of your API's data and the right to create, read, update and delete any of the data that you see fit (but we hope you don't do that while in production!)  

Go to the [Manage Section](https://drawpi.com/dashboard/manage), and select the Project whose code you want to download. A dropdown will expand below the selected project in the left Sidebar. Click on **DB Schema**.  
Select the table that you want to manage.  

![Imgur](https://i.imgur.com/GCRticR.png)

#### Rows

You can manage your table data in the rows section.
Add, Update, Delete data in your table which is safely stored in the DrawPI database.

![Imgur](https://i.imgur.com/LGI5lzT.png)

#### Columns

You can also manage the table attributes.
Add column attributes or change their default values or datatypes.
> **Note**: Make sure the integrity of the table data is preserved before making the changes. For example, if you try to change a column datatype from varchar to int, which has already varchar data inside the table, this change will fail to apply.

![Imgur](https://i.imgur.com/l24UoBA.png)