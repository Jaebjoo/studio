---
title: Studio 6 
layout: default
description: Resource Locks
---

## Studio 6 : 
# Resource Locks

#### Azure Learn

https://docs.microsoft.com/en-au/learn/modules/build-cloud-governance-strategy-azure/6-protect-storage-account-resource-lock

Resource locks help prevent accidental deletion of your Azure resources.
It is important that human error is avoided with administration.
It is important to differntiate resources which are vital to the organisation and need to be protected.
Accidental deletions could possibly occur when cleaning up a resource group, inadvertently removing an essential service.

**Resource lock can be added to resource groups as well as individual resources.**

**We have added a resource lock to the ICTHelpDesk Resource Group to protect it from accidental deletion and also to demonstrate the use of this function**

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 7.57.53 PM.png "Image")

First a new resource group will be created in this exercise to demonstrate this function.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 7.58.09 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 7.58.23 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 7.59.06 PM.png "Image")

Under settings, there is a locks option.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 7.59.26 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 7.59.32 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 7.59.40 PM.png "Image")

You can add a name to the lock to specify what is is for.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 7.59.47 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.00.01 PM.png "Image")

The lock will be a delete type lock which blocks deleting of this resource.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.00.14 PM.png "Image")

The scope will cover the entire resource group.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.00.35 PM.png "Image")

I will try to delete this resource group after adding a lock.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.00.40 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.00.53 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.00.57 PM.png "Image")

The delete action is blocked by the resource lock and a message mentioning which lock has blocked this action is displayed.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.01.06 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.01.40 PM.png "Image")

A storage account has been added to this resource group.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.02.22 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.03.45 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.03.49 PM.png "Image")

The delete will fail as the lock restriction extends to all resources within the resource group.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.03.52 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.04.30 PM.png "Image")

We will remove the resource lock.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.04.32 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.04.36 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.04.47 PM.png "Image")

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.04.53 PM.png "Image")

The deletion has been successful affter the lock has been removed.

![Image](images\Protect a storage account from accidental deletion by using a resource lock\Screen Shot 2021-01-22 at 8.06.46 PM.png "Image")
