---
title: Studio 6 
layout: default
description: Timer Trigger
---

## Studio 6 : 
# Timer Trigger

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/execute-azure-function-with-triggers/4-create-timer-trigger?pivots=csharp

**Timer triggers run the Azure function code at a scheduled time.**

The example given is a blog owner who notices that their subscribers aren't reading your most recent posts. You decide that the best action is to send an email once a week to remind them to check your blog. You implement this logic using an Azure function app with a timer trigger to invoke your function weekly.

**It is based on a CRON expression.**

**The order of six fields is 
{second} {minute} {hour} {day} {month} {day of the week}.**

You must first create a Function App which can be found in the marketplace.

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.27.33 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.27.38 PM.png "Image")

**The following are the configuration details.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.28.34 PM.png "Image")

**It is to be hosted on Windows system, and serverless.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.29.28 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.31.55 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.32.03 PM.png "Image")

**Functions code is stored in the functions section.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.32.18 PM.png "Image")

**You add a timer trigger following this process.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.32.24 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.32.49 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.33.12 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.33.15 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.33.33 PM.png "Image")

**Function timer trigger has been created.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.34.19 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.34.30 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.34.40 PM.png "Image")

**You can edit the timer trigger and schange the schedule.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.34.46 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.35.12 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.35.16 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.35.26 PM.png "Image")

**The demo code is to simply display log information to confirm trigger execution.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.35.36 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.35.58 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.36.21 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.36.36 PM.png "Image")

**You can run the code.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.36.46 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.37.10 PM.png "Image")

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.37.22 PM.png "Image")

**The trigger can be checked in the logs display.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.37.48 PM.png "Image")

**Function has been disabled to end this demo.**

![Image](images\Create a timer trigger\Screen Shot 2021-02-15 at 9.37.54 PM.png "Image")