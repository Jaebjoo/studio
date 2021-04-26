---
title: Studio 6 
layout: default
description: Azure Lab Services
---

## Studio 6 : 
# Azure Lab Services

#### Research Summary

https://azure.microsoft.com/en-us/services/lab-services/#overview

Azure Lab Services allows creation of classroom resources such as virtual machines with a friendly interface.
Students can be invited to a particular "lab" or classroom. 
Students can then be assigned resources individually.
Resources can be managed, shutdown and deleted no the Lab Services Platform.

The running times of resources could be scheduled and also restricted so that the resource would only be running while it is in use and within a predetermined time period.

Azure Lab Services would therefore help avoid cost overruns and allow administrators to view costs incurred for each "lab"/class.

Students could be added using a csv file.
This would have been very useful as the student details could be obtained from the Student Adminsitration at OP.

Rohill and I made a request to make a Azure Lab Services resource

![Image](images\AzureLabServices\Screenshot 2021-04-26 143250.png "Image")

However we soon realised that VMs that are cost efficient, costing approxiamtely between 7- 14 NZD were not available on this platform.
This solution was quickly abandoned.

However we were able to explore the possibilities with the creation of template VMs and replicating them for a classroom.

It would be easy for lecturers to interact with the platform interface to create, allocate and manage resources.

Unfortunately due to budget constraints, this would not be viable.

Rob and I did discuss creating single Lab Services resource structured under resource groups for each theme off IT (web/admin/programming/db) and creating individual "labs"/classes within them.

Until Microsoft offers cheaper VMs on this platform, BIT will have to create VMs directly on the Azure Infrastructure.