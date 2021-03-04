---
title: Studio 6 
layout: default
description: ICT Helpdesk Migration
---

## Studio 6 : 
# ICT Helpdesk Migration

#### Client's Requests

Job assigned **March 1**

Due Date **April 9**

Rob requires the ICT helpdesk site (https://help.ict.op.ac.nz) to be migrated from the current server (fthictweb08@ict.op.ac.nz) to the Azure infrastructure.
the ICT helpdesk website contents are currently being stored in a GitHub repository.

![Image](images\ICT Helpdesk Migration\Screenshot 2021-03-04 144915.png "Image")

#### Summary

Task in progress...

#### Reflection

* **Research** + Learning - Gained understanding of a new Azure Resource (Static Web App) for hosting a simple website.
This is a lightweight PaaS solution opposed to a IaaS solution with a VM and web hosting software.

* **Communication** - Communication with teammate (Rohill) was effective and coordination was well executed.
Liason with Rob and Faisal was timely and concise. We reported our progress as much as possible and consulted Rob about the possible solution.

* **Documentation** - A Proposal Report documenting the summary of research was created. Further documentation about the Static Web App migration was created and store on the DevOps Team Documentation for future reference.

* **Time Management** - 

Task in progress...

#### Worklog

Working with **Rohill Nand**

###### March 1

The website needs a simple web hosting platform solution. A separate VM is too heavy for a small website.
Azure Cloud Service provides **Azure Static Web App** Resource which allows hosting of a website which can also be linked to a GitHub Repository.

**Azure Static Web App Diagram**

![Image](images\ICT Helpdesk Migration\Screen Shot 2021-03-02 at 10.16.14 PM.png "Image")

Research was conducted and Azure Static Web App was determined to be the best solution as it is lightweight and free.
A small linux VM was a unfavourable alternative.

**Resource Creation Fail**

![Image](images\ICT Helpdesk Migration\StaticWebApp Resource Creation Fail.png "Image")

ICT Helpdesk resource group was allocated to Rohill and I by Faisal.
However we did not have permissions to create a new static web app resource.
Faisal requested a proposal report to justify the possible solution.

###### March 4

Rohill and I drafted a solution Proposal report and submitted it to Faisal and Rob.

**Solution Proposal**

![Image](images\ICT Helpdesk Migration\Screenshot 2021-03-04 143548.png "Image")

We received approval of the solution from Rob.

![Image](images\ICT Helpdesk Migration\Screenshot 2021-03-04 150651.png "Image")

However we need to create the Static Web App resource with Rob's authorisation level.

![Image](images\ICT Helpdesk Migration\Screenshot 2021-03-04 150730.png "Image")

###### March 8

** Planning to start building the website after resource creation with Rob...