---
title: Studio 6 
layout: default
description: Azure Fundamentals 1
---

## Studio 6 : 
# Azure Fundamentals 1 - What is Cloud Services?

#### Azure Research

https://docs.microsoft.com/en-us/learn/paths/az-900-describe-cloud-concepts/

Understanding the different levels of cloud resources have been applied in the OP Migration. It is most often more convenient to migrate resources as a PaaS rather than a IaaS. Although, there is a trade off of having more control, it is more lightweight and less maintenance.

Understanding ofResource groups, subscriptions and management groups are also essential in organising the resources. This is key for a Cloud administrator. It has also been apparent in STUDIO6 that TAGS are essential with resources.

In terms of Azure regions, DevOps has limited its region to South East Australia and Asia region.

## Benefits of Cloud Computing

The key benefits of cloud environment over physical environment are:

* **Reliatility** - reducing the risk of downtime with faults in physical machines. The burdens of managing physical devices are offloaded to the cloud service provider.

* **Scalability** - Resources can be scaled automatically VERTICALLY increasing the capacity of the single resource, or HORIZONTALLY by increassing the instances of a particular resource. These can be added according to the needs of the business.

* **Elasticity** - An organisation can configure only the resources they need.

* **Agility** - Cloud resources can be deployed quickly, responding to changes in resource demands.

* **Geo-distribution** - Applications can be hosted globally in particular regions.

* **Disaster recovery** - With data replication and geo-distribution, you can have a contingency plan in the event of a disaster.

## Different Categories of Cloud Services

![Image](images\AF1\Screenshot 2021-03-16 213353.png "Image")
![Image](images\AF1\Screenshot 2021-03-16 213413.png "Image")

* **IaaS** - A cloud provider keeps the hardware up to date, but operating system maintenance and network configuration is left to the cloud tenant. For example, Azure virtual machines are fully operational virtual compute devices running in Microsoft's datacenters. An advantage of this cloud service model is rapid deployment of new compute devices. Setting up a new virtual machine is considerably faster than procuring, installing, and configuring a physical server.

* **PaaS** - This cloud service model is a managed hosting environment. The cloud provider manages the virtual machines and networking resources, and the cloud tenant deploys their applications into the managed hosting environment.

* **SaaS** - In this cloud service model, the cloud provider manages all aspects of the application environment, such as virtual machines, networking resources, data storage, and applications. The cloud tenant only needs to provide their data to the application managed by the cloud provider.

## Different Types of Cloud Computing

![Image](images\AF1\Screenshot 2021-03-16 213442.png "Image")

* **Public Cloud** - Services are offered over the public internet and available to anyone who wants to purchase them. Cloud resources like servers and storage are owned and operated by a third-party cloud service provider and delivered over the internet.

* **Private Cloud** - Computing resources are used exclusively by users from one business or organization. A private cloud can be physically located at your organization's on-site datacenter. It also can be hosted by a third-party service provider.

* **Hybrid Cloud** - This computing environment combines a public cloud and a private cloud by allowing data and applications to be shared between them.