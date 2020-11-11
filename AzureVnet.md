---
title: Studio 5 Azure Vnet
layout: default
description: Studio 5 Azure VNet
---

## Studio 5 : 
# Azure VNet

#### Research Summary

Azure Virtual Networks are easy to deploy, however considerations on Network Design should be thoroughly planned beforehand.

Creating Virtual Switches using Hyper-V Manager is also possible.

VMs are able to have restricted access from the public network and only gain access through a gateway VM.

Vnets can be interconnected using Peering.
Subnets can also be easily created within Azure.

Different conffigurations are possible with VMs able to attach 2+ Network adaptors. Bridging on a gateway VM was attempted but not completed.

Several Factors need to be considered while Planning virtual networks. These include:

* Naming
* Region
* Subscription
* Security
* Connectivity
* Permissions

Connectivity is limited across several regions, so it is imperative to check that all necessary resources are available and offered by Azure in a particular region before deployment.

Network Security groups can easily limit who has access to resources on a network and permissions can restrict that scope according to a entity's hierarchy.