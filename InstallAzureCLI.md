---
title: Studio 6 
layout: default
description: Install and run the Azure CLI
---

## Studio 6 : 
# Install and run the Azure CLI

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/control-azure-services-with-cli/3-exercise-install-and-run-the-azure-cli?pivots=macos

**The Azure CLI is a command-line program to connect to Azure and execute administrative commands on Azure resources.** It runs on Linux, macOS, and Windows and allows administrators and developers to execute their commands through a terminal or command-line prompt (or script!) instead of a web browser.

Learning how to use this tool will be useful for scripts and navigating through the Azure infrastructure quickly without the Portal.

**The deployment of the website below is also potentially a solution for the ICT Helpdesk Website**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.34.50 PM.png "Image")

**Update your brew repository to make sure you get the latest Azure CLI package**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.35.50 PM.png "Image")

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.36.12 PM.png "Image")

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.39.44 PM.png "Image")

**Install the Azure CLI**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.41.15 PM.png "Image")

**Start the Azure CLI and verify your installation by running the version check**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.41.54 PM.png "Image")

**These are some example commands that can be used on the CLI**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.43.07 PM.png "Image")

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.48.51 PM.png "Image")

**create several variables that you will use in later commands**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.48.58 PM.png "Image")

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.49.13 PM.png "Image")

**Create an App Service plan to run your app. The following command specifies the free pricing tier, but you can run az appservice plan create --help to see the other pricing tiers**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.50.00 PM.png "Image")

**Verify that the service plan was created successfully by listing all your plans in a table**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.50.28 PM.png "Image")

**To create the web app, you'll supply web app name and the name of the app plan you created above. Just like the app plan name, the web app name must be unique, and the variables that you created earlier will assign random values that should be sufficient for this exercise**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.53.24 PM.png "Image")

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.58.14 PM.png "Image")

**use curl command to see the contents of created website**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 2.58.58 PM.png "Image")

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 3.00.53 PM.png "Image")

**The final step is to deploy code from a GitHub repository to the web app. Let's use a simple PHP page available in the Azure Samples GitHub repository that displays "Hello World!" when it executes. Make sure to use the web app name you created**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 3.02.40 PM.png "Image")

**This is the original default page before deployment**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 3.02.44 PM.png "Image")

**The manual deployment from GitHub is being processed**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 3.02.57 PM.png "Image")

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 3.03.26 PM.png "Image")

**Once the deployment has finished from the master branch of the repository, we can confirm with curl command or use the browser**

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 3.03.46 PM.png "Image")

![Image](images\Install and run the Azure CLI\Screen Shot 2021-02-09 at 3.03.54 PM.png "Image")