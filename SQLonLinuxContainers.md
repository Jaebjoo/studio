---
title: Studio 6 
layout: default
description: SQLonLinuxContainers
---

## Studio 6 : 
# Run SQL Server 2019 on Linux containers

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/run-sql-server-2017-linux-containers/3-create-custom-images

In SQL Server 2019, you can choose to run a database server on Linux or Windows. Also, you can decide to run a database on a physical server, or in a virtual environment like a Virtual Machine (VM) or a container.

Suppose you want to make it easier to deploy database servers into the testing environment for your photo-sharing application. You need to provide clean sample databases for integration and acceptance testing as quickly as possible. Because the production environment is hosted on Linux servers, you want the testing environment to run Linux too.

**DB3 resources will include SQL Docker containers for Students to maintain.**

It will be important to understand these procedures to setup SQL docker containers to participate in creating that Azure Service.

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.53.23 PM.png "Image")

**Create a random password and use it when creating a Ubuntu Server VM**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.55.16 PM.png "Image")

**The Ip address of the VM is stored in a variable**

**The password of the VM is as follows**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.56.52 PM.png "Image")

**Use this information to SSH to the VM**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.57.11 PM.png "Image")

**Run an update and install packages that allow apt to use a repository over HTTPS, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.57.44 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.57.46 PM.png "Image")

**To add the Docker GPG key, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.58.16 PM.png "Image")

**To add install packages that allow apt to use a repository over HTTPS, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.58.28 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.58.39 PM.png "Image")

**Update and install Docker, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.58.49 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.59.27 PM.png "Image")

**When installation is complete, check the status of the Docker service**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.59.31 PM.png "Image")

**To automatically start Docker when the system boots up, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.59.42 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.59.49 PM.png "Image")

**Now we have a Linux VM and docker installed, in the terminal, to pull the SQL Server container image, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 9.59.56 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.00.29 PM.png "Image")

**In the terminal, to run the SQL Server container image, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.03.20 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.03.30 PM.png "Image")

**When the image is downloaded and the container started, you check that SQL Server is running in the new container. Type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.03.38 PM.png "Image")

**In the Cloud Shell, To start the bash shell within the new container, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.03.50 PM.png "Image")

**To start the sqlcmd tool, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.04.13 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.04.19 PM.png "Image")

**You are now in SQL inside the container. To query the database server, type the following commands, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.04.34 PM.png "Image")

**List all container images**

**Stopping the container**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.05.36 PM.png "Image")

**You can check the container has stopped with "sudo docker ps -a"**

**We will also remove the container**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.05.51 PM.png "Image")

**You can automate the startup of multiple Docker images by using a container orchestrator package, such as Docker Compose.**

**To download Docker Compose, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.07.08 PM.png "Image")

**To mark the downloaded file as executable, type the following command, and then press Enter**

**To create a link to the downloaded executable, type the following command, and then press Enter**

**In the Cloud Shell on the left, to clone the GitHub repo in the Ubuntu VM, run this command**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.07.30 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.07.57 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.09.15 PM.png "Image")

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.09.29 PM.png "Image")

**In the terminal, type the following command, and then press Enter**

![Image](images\Run SQL Server 2019 on Linux containers\Screen Shot 2021-02-02 at 10.11.17 PM.png "Image")