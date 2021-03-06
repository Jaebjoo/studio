---
title: Studio 6 
layout: default
description: Function App
---

## Studio 6 : 
# Create a function app in the Azure portal

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/create-serverless-logic-with-azure-functions/3-create-an-azure-functions-app-in-the-azure-portal?pivots=javascript

**Functions are hosted in an execution context called a function app. You define function apps to logically group and structure your functions and a compute resource in Azure.**

Essentially, Azure allows you to use Functions app to run, code, logic without a VM.

You can find Functions App in the Marketplace.

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 7.52.47 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 7.52.59 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 7.53.04 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 7.54.22 PM.png "Image")

**Functions can be triggered to run upon a certain event, and also have bindings which are data input and output connections from a source or destination.**

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 7.57.31 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 7.58.35 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.07.30 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.07.36 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.07.42 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.07.59 PM.png "Image")

**In this example we will add a HTTP trigger, that will trigger the function with a HTTP request.**

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.08.15 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.08.22 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.08.27 PM.png "Image")

**You can view the code for this HTTP Trigger here**

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.08.58 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.09.02 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.09.23 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.10.37 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.10.48 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.14.58 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.15.01 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.15.05 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.15.27 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.15.31 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.16.32 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.17.12 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.17.17 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.17.22 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.18.19 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.18.50 PM.png "Image")

**In this example code, the function will have readings for devices and display a message corresponding to the temperature readings**

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.33.49 PM.png "Image")

**We will pass the following Readings as a POST**

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.33.56 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.34.00 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.34.10 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.34.20 PM.png "Image")

**When this POST was processed by the function, which triggered with the POST request, the messages corresponding to the temperature readings were displayed.**

**This can be further extended with output bindings if required to send data to a database holding the status of all devices.**

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.34.28 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.34.32 PM.png "Image")

**The function works successully**

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.34.52 PM.png "Image")

![Image](images\Create a function app in the Azure portal\Screen Shot 2021-01-31 at 8.35.20 PM.png "Image")