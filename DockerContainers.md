---
title: Studio 6 
layout: default
description: Docker Containers
---

## Studio 6 : 
# Docker Containers

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/run-docker-with-azure-container-instances/

Containers offer a standardized and repeatable way to package, deploy and manage cloud applications. Azure Container Instances let you run a container in Azure without managing virtual machines and without a higher-level service.

**This option may apply to the Linux Course resources that needed for Faisal.**

Container networking must be futher researched.

However in this demp, container instance is created rather than within a VM.

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.47.38 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.47.43 PM.png "Image")

**Create a new resource group with the name learn-deploy-aci-rg**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.49.00 PM.png "Image")

**You provide a DNS name to expose your container to the Internet.**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.49.06 PM.png "Image")

**Run the following az container create command to start a container instance.**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.49.10 PM.png "Image")

**Run az container show to check its status**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.49.24 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.49.29 PM.png "Image")

**From a browser, navigate to your container's FQDN to see it running. You see this**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.49.36 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.49.50 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.49.54 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.00 PM.png "Image")

**Azure Container Instances starts the container and then stops it when its process (a script, in this case) exits. When Azure Container Instances stops a container whose restart policy is Never or OnFailure, the container's status is set to Terminated.**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.07 PM.png "Image")

**Run az container show to check your container's status**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.17 PM.png "Image")

**View the container's logs to examine the output. To do so, run az container logs like this**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.24 PM.png "Image")

**You see this**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.29 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.36 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.44 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.48 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.50.57 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.04 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.08 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.12 PM.png "Image")

**Once the app is available, you see this**

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.21 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.28 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.32 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.37 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.41 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.46 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.51.58 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.00 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.04 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.07 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.11 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.14 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.17 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.19 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.25 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.31 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.38 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.40 PM.png "Image")

![Image](images\Run Docker containers with Azure Container Instances (re-do with own subscription)\Screen Shot 2021-01-31 at 8.52.44 PM.png "Image")