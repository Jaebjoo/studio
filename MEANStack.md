---
title: Studio 5 
layout: default
description: Build and run a web application with the MEAN stack on an Azure Linux virtual machine
---

## Studio 5 : 
# Build a MEAN Stack on Linux virtual machine

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/build-a-web-app-with-mean-on-a-linux-vm/

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.32.58 PM.png "Image")

A Linux machine is created with the following command on Azure CLI

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.33.14 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.33.33 PM.png "Image")

Status message is shown once the VM has been created.

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.34.49 PM.png "Image")

Port 80 must be opened using the following command. This is to allow incomming HTTP traffic.

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.35.06 PM.png "Image")

Store the ip address of the vm "MeanStack" into variable "ipaddress" using following command. 

ssh to the VM using ip address with the user "azureuser"

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.35.42 PM.png "Image")

ssh to VM is successful.

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.38.02 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.39.05 PM.png "Image")

Run updates on the VM

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.39.40 PM.png "Image")

Install MongoDB using apt-get command

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.39.53 PM.png "Image")

Check that Mongo DB is running

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.40.36 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.40.54 PM.png "Image")

Check version of MongoDB

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.41.56 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.42.08 PM.png "Image")

Register the Node.js repository so package manager can locate the packages

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.42.39 PM.png "Image")

Install the Node.js package

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.47.26 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.47.45 PM.png "Image")

verify installation using 'nodejs -v' command. This version is v.4.2.6

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.47.55 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.48.00 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.48.21 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.49.06 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.49.12 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.50.23 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.50.44 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.51.06 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.51.13 PM.png "Image")

Start coding with 'code' command.

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.51.48 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.52.14 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.52.36 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.53.14 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.54.07 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.54.32 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.54.41 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.54.51 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.54.54 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.55.12 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.55.24 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.55.32 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.55.50 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.55.54 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.56.16 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.56.19 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.56.29 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.56.46 PM.png "Image")

Move the completed code directory to the VM

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.56.52 PM.png "Image")

ipaddress of VM. SSH to VM

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.57.58 PM.png "Image")

Books directory has been received with scp

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.58.07 PM.png "Image")

change directory into Books and sudo apt install npm

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.58.20 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 9.58.52 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.05.36 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.05.46 PM.png "Image")

Start the web application

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.06.03 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.06.32 PM.png "Image")

Type ip address on web browser to go to web application being served on VM

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.06.37 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.06.50 PM.png "Image")

Adding a book on the web application

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.07.21 PM.png "Image")

Successfully added

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.07.28 PM.png "Image")

VM responds with addition on Mongo

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.07.34 PM.png "Image")

Deleting the Record

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.07.44 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.07.53 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.07.56 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.08.01 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.08.34 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.08.37 PM.png "Image")

![Image](images\Build and run a web application with the MEAN stack on an Azure Linux virtual machine\Screen Shot 2021-01-25 at 10.08.42 PM.png "Image")
<!-- ![Image](images\Linux_Configuration\4vnet3peering.png "Image") -->
