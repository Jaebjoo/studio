---
title: Studio 6 
layout: default
description: Azure Fundamentals 2
---

## Studio 6 : 
# Azure Fundamentals 2 - Azure Resources

#### Azure Research

https://docs.microsoft.com/en-us/learn/paths/az-900-describe-core-azure-services/

Azure offers a variety of resources ranging from Databases, Computing, Disk storage, Big Data Analytics and these resources are connected with Azure Networking. 

Understanding and being aware of the services available allows DevOps team to recommend and provide the most appropriate resources for a solution to a customer.

Understanding Databases were important for assisting Krissi and understanding computing options were important for Linux Course resources for Faisal.

## Databases and Analytics on Azure

Various Database platform options are available on Azure.
These DB can be connected to Azure ML and Analytic services to generate relevant information to assist business decision.

Azure Cosmos DB is a globally distributed, multi-model database service. You can
elastically and independently scale throughput and storage across any number of
Azure regions worldwide.
Highly responsive and Always on.
* Flexible
* Stores data in Atom-record-sequence ARS

## SQL Database.

![Image](images\AF2\Screenshot 2021-03-16 214756.png "Image")

Various Databases can be created as IaaS or PaaS model:
* **MYSQL** - a relational database service in the cloud, and it's based on the MySQL Community Edition database engine, versions 5.6, 5.7, and 8.0

![Image](images\AF2\Screenshot 2021-03-16 214817.png "Image")

* PostgreSQL - a relational database service in the cloud. The server software is based on the community version of the open-source PostgreSQL database engine.

## Azure Analytics

There are various big data and analytics services on microsoft Azure which can process the large datasets that have been collected by an organisation in their Databases.

* Azure Synapse Analytics
* Azure HDInsight
* Azure Databricks
* Azure Data Lakes Analytics

Compared to having Databases on-premise, cloud resources on Azure allow Synergy with Azure Analytics.

## Azure Compute Services

There are various computing resources that are available on Azure.

* Azure VM
* Azure Container Instances
* Azure App Service
* Azure Functions

With Azure Virtual Machines, you can create and use VMs in the cloud. VMs provide infrastructure as a service (IaaS) in the form of a virtualized server and can be used in many ways. Just like a physical computer, you can customize all of the software running on the VM. VMs are an ideal choice when you need:
* Total control over the operating system (OS).
* The ability to run custom software.
* To use custom hosting configurations.

Azure App Services and Functions are not Infrastructure services. They allow lightweight solutions that are low maintenance.

These computing resources allow:

* During Testing and Development.
* Running application on Cloud
* Extending datacentre into cloud
* During Disaster recovery
* Windows Virtual Desktop

## Azure Storage

Azure Storage Resources include: 

* Azure Blob Storage
* Azure Disk Storage
* Azure Files Storage
* Azure Blob Access Tiers

These are organised as such.

**Account >> Container >> Blob**

Storages can hold any sort of files or data.
These storages can be flexibly scaled as needed.

## Networking

Virtual Networking

* Isolation / Segmentation
* Internet Communications
* Communicate between Azure resources
* Communicate with on-premise resources

Azure networks can be divided and peered so different networks can communicate with each other. 

![Image](images\AF2\Screenshot 2021-03-16 223634.png "Image")

Azure networks work similarly with general networks:
* Route network traffic
* Filter network traffic
* Connect Virtual Networks

VPNs can enable branch offices to share sensitive information between locations.

Network Security Groups can be configured to block or allow traffic and also manage ports.

![Image](images\AF2\Screenshot 2021-03-16 223644.png "Image")

All transferred data is encrypted in a private tunnel as it crosses the internet.