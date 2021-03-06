---
title: Studio 6 
layout: default
description: Input Binding Types
---

## Studio 6 : 
# Input Binding Types

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/chain-azure-functions-data-using-bindings/5-read-data-with-input-bindings-portal-lab?pivots=javascript

**Input binding is a connection from a Source such as a blob storage, Azure DB, Mobile Apps, Table storage.**

In this demo, the function app will take data from Azure DB.

The following are the steps taken to create a Azure Cosmos DB Account.

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.22.55 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.24.21 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.24.44 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.24.55 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.27.44 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.27.52 PM.png "Image")

**A new container is created to hold data**

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.28.11 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.28.25 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.28.58 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.29.04 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.30.05 PM.png "Image")

**The new container is to hold Bookmarks**

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.30.44 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.42.17 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.42.21 PM.png "Image")

**We will create a new item which has a microsoft Azure URL.**

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.42.31 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.42.45 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.44.19 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.45.10 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.45.13 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.45.16 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.45.18 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.46.29 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.46.54 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.47.59 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.49.37 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.49.47 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.49.56 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.50.07 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.51.35 PM.png "Image")

**Under the function that was created we will add a input binding.**

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.52.21 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.54.23 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.54.35 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.54.44 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.54.50 PM.png "Image")

**If the document id in the url is in the HTTP request and it is held in the DB, it will display the URL**

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.55.41 PM.png "Image")

**we will pass the id of "docs"**

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 10.56.25 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 11.06.39 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 11.06.46 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 11.06.53 PM.png "Image")

**The docs bookmark URL has been displayed**

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 11.07.05 PM.png "Image")

![Image](images\Read data with input bindings\Screen Shot 2021-02-15 at 11.07.10 PM.png "Image")

**The azure bookmark URL has been displayed**