---
title: Studio 6 
layout: default
description: PostgreSQL VM Request
---

## Studio 6 : 
# PostgreSQL VM Request (David)

#### Client's Requests

Job assigned **April 4**

Due Date **April 14**

Job Completed **April 8**

https://azure.microsoft.com/en-us/services/postgresql/

![Image](images\PostgreSQLVM\Screenshot 2021-04-26 144456.png "Image")

Cody Smith from David's Studio Team approaced us with a request for a PostgreSQL server and a Web server.

We looked into the possiblity of supplying them with a PaaS option, however the PaaS option for both PostgreSQL and Web hosting was quite expensive. costing $~50 per month for each. Though we do have a budget, the resource would not be cost efficient and too heavy for the task.

We looked for a simpler option of creating a lighter Linux VM at the cost of $15.30 NZD per month.

![Image](images\PostgreSQLVM\Screenshot 2021-04-26 144542.png "Image")

We installed the necessary PostgreSQL service onto the VM, and also made sure that the only ports open would be 22 and 5432 which is for postgresql.
The team will most likely need 8080 and 443 later for the Webserver, and will probably use Django or Apache to be serving their web app.

The password credentials were passed onto the team and the password was also stored on our KeyPass file stored on Teams.

The details of the resource was also logged into the Azure Resources OneNote on Teams.

This was a good chance for the DevOps team to be involved with providing development resources for Studio teams and it would be great to have more collaboration in this manner.


