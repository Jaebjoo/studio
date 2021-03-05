---
title: Studio 6 
layout: default
description: Restrict deployments to a specific location by using Azure Policy
---

## Studio 6 : 
# Restrict deployments to a specific location by using Azure Policy

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/build-cloud-governance-strategy-azure/9-restrict-location-azure-policy

Azure Policy restricts the deployment of Azure resources to a specific location. You verify the policy by attempting to create a storage account in a location that violates the policy.

Limiting the deployment region can:

* improve cost tracking
* adhere to data residency and security compliance according to government regulations.

**This feature can be applied in OP and Studio DevOps team to restrict deployment of resources to Australia or at least Asia region.**

**This can also limit the size of VMs or other costly resources that could be accidentally created by unsupervised students.**

This demo will only cover regional restrictions of resource deployments.

**Such accidental deployments in the US region have occured in the previous semester.**

It is important that policies are discussed and set with Rob and Faisal to limit the potential mistakes that can occur.

A resource group will be created to demonstrate this function.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.11.01 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.11.18 PM.png "Image")

Azure Policies can be navigated to from HOME.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.12.13 PM.png "Image")

There are definitions which define the scope of the policies.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.12.46 PM.png "Image")

Compute will be selected.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.13.28 PM.png "Image")

We will select allowed VM size.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.13.42 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.13.49 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.13.58 PM.png "Image")

The policy assignment will affect the new resource group.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.14.41 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.14.45 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.15.28 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.15.58 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.16.10 PM.png "Image")

The new policy will restrict the allowed locations and also detail who it has been assigned by.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.17.23 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.17.27 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.17.31 PM.png "Image")

Under parameters, the allowed regions can be defined.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.17.42 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.18.00 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.18.35 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.18.58 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.19.02 PM.png "Image")

We will attempt to create a storage account outside the scope of the policies set. In this case it will be in East US.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.19.05 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.19.20 PM.png "Image")

The deployment has failed.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.19.34 PM.png "Image")

The summary of the deployment error specifies that it has been disalllowed by a particular policy. 

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.19.51 PM.png "Image")

We will delete the assignment of the policy and reattempt the deployment in East US.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.20.18 PM.png "Image")

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.20.41 PM.png "Image")

Deployment has succeeded.

![Image](images\Restrict deployments to a specific location by using Azure Policy\Screen Shot 2021-01-22 at 8.21.37 PM.png "Image")