---
title: Studio 6 Static Web App
layout: default
description: Studio 6 Static Web App
---

## Studio 6 : 
# Static Web App

#### Research Summary

https://azure.microsoft.com/en-us/services/app-service/static/

![Image](images\StaticWebApp\Screenshot 2021-03-04 153137.png "Image")

Azure Static Web Apps publishes a website to a production environment by building apps from a GitHub repository. In this quickstart, you deploy a web application to Azure Static Web apps using the Visual Studio Code extension.

When you create an Azure Static Web Apps resource, Azure sets up a GitHub Actions workflow in the app's source code repository that monitors a branch of your choice. Every time you push commits or accept pull requests into the watched branch, the GitHub Action automatically builds and deploys your app and its API to Azure.

With Static Web Apps, static assets are separated from a traditional web server and are instead served from points geographically distributed around the world. This distribution makes serving files much faster as files are physically closer to end users. In addition, API endpoints are hosted using a serverless architecture, which avoids the need for a full back-end server all together.

![Image](images\ICT Helpdesk Migration\Screen Shot 2021-03-02 at 10.16.14 PM.png "Image")

I found this to be a solution to host the ICT Helpdesk Website. This is a PaaS solution.
The alternative to this would be to run a VM, which is resource intensive relative to the task.

