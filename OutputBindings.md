---
title: Studio 6 
layout: default
description: Output Bindings
---

## Studio 6 : 
# Output Bindings

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/chain-azure-functions-data-using-bindings/7-write-data-with-output-bindings-portal-lab?pivots=javascript

**Output bindings of functions are destinations for data.** There are numerous binding types which include blob storage, HTTP, microsoft graph and mobile apps.

**Functions will create connection between apps and data storage.**

In this demo, there will be a HTTP request to add a bookmark.

If this bookmark is not in the DB already, it will add the bookmark and display an appropriate response.

If this bookmark already exist, it will display a response accordingly.

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.08.19 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.09.09 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.09.12 PM.png "Image")

**We will create an output binding to the Cosmos DB created.**

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.10.01 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.13.18 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.13.24 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.15.33 PM.png "Image")

**This is the demo code, if it exists then the message "Bookmark exists will display, otherwise it will create a JSON String and write it to the database.**

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.15.38 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.16.21 PM.png "Image")

**We will test this function with a POST. The id is docs and url is the Azure page.**

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.16.54 PM.png "Image")

**Error message displays**

**We will try a different POST request with GitHub Home.**

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.17.06 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.17.19 PM.png "Image")

**We will check the DB to see if the entry has been made**

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.17.25 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.17.30 PM.png "Image")

**It has been added**

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.18.09 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.18.14 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.18.16 PM.png "Image")

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.18.19 PM.png "Image")

**A message has been posted in logs.**

![Image](images\Write data with output bindings\Screen Shot 2021-02-15 at 11.18.25 PM.png "Image")