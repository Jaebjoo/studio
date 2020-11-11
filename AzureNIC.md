---
title: Studio 5 Azure NIC
layout: default
description: Studio 5 Azure NIC
---

## Studio 5 : 
# Azure NIC

#### Research Summary

A brief exploration into Network interface restrictions revealed that the size of the VM will determine how many network adaptors can be added. Further details are specified in the Linux Configuration page. 

VMs capable of attaching upto 4 Network Adapters cost from 200 NZD per month to operate.

VMs usually have a limit of 2.
Obviously VMs when created are configured to have 1 attached. An additional NI can be connected in the network settings of the VM. 
NI can be customised with a unique name and also managed seperately within the Vnet settings.

Though I am not aware of what the wider potential of having multiple Network adapters is, opposed to simply being connected via Vnet and Peering, it should allow unique network topologies in a corporate environment.