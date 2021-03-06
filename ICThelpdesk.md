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

Job Completed **March 8** (deployed)

Rob requires the ICT helpdesk site (https://help.ict.op.ac.nz) to be migrated from the current server (fthictweb08@ict.op.ac.nz) to the Azure infrastructure.
the ICT helpdesk website contents are currently being stored in a GitHub repository.

![Image](images\ICT Helpdesk Migration\Screenshot 2021-03-04 144915.png "Image")

#### Summary

**The ICT Helpsite has been successfully migrated to the Azure Infrastructure with a Static Web App.**

It has been connected to the Github Repository.

It requires a content update in the long run. However the job has been completed.

**This solution is a good template for any projects that need to be hosted on the Azure Infrastructure.**

#### Reflection

* **Research** + Learning - Gained understanding of a new Azure Resource (Static Web App) for hosting a simple website.
This is a lightweight PaaS solution opposed to a IaaS solution with a VM and web hosting software.

* **Communication** - Communication with teammate (Rohill) was effective and coordination was well executed.
Liason with Rob and Faisal was timely and concise. We reported our progress as much as possible and consulted Rob about the possible solution.

* **Documentation** - A Proposal Report documenting the summary of research was created. Further documentation about the Static Web App migration was created and store on the DevOps Team Documentation for future reference.

* **Time Management** - The job was completed in a short period of time with good research and implementation. We knew enough of how to execute the deployment to do so without much problems. The process of creating the static web app and deploying the github repository was very straightforward.

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

Meeting with Rob to create the Static Web App.

**There is a tutorial on the Microsoft Website about creating the resource**

![Image](images\ICT Helpdesk Migration\1.png "Image")

**These are the example configurations for the creating of the Static Web App resource**

![Image](images\ICT Helpdesk Migration\2.png "Image")

**You must sign in with GitHub and choose the easysdadmin organisation and ICTHelp repository, the branch is the Master**

![Image](images\ICT Helpdesk Migration\3.png "Image")


**There are build settings for the static web app**

**This is what is needed for HUGO build settings, however we only realised this after creating the resource**

![Image](images\ICT Helpdesk Migration\4.png "Image")

**This new file was created by microsoft static apps and commited to the github repository**

**We need to note the output location: "dist" line at the bottom**

![Image](images\ICT Helpdesk Migration\5.png "Image")

**GitHub attempts to build the website**

![Image](images\ICT Helpdesk Migration\6.png "Image")

**However this build and deploy fails.**

![Image](images\ICT Helpdesk Migration\7.png "Image")

**This was the error message in the GitHub Actions page.**

![Image](images\ICT Helpdesk Migration\8.png "Image")

**This is where we realised thaat the platform was HUGO. The build process automatically detects this.**

![Image](images\ICT Helpdesk Migration\9.png "Image")

**For HUGO we changed the output location to be "public"**

![Image](images\ICT Helpdesk Migration\10.png "Image")

**There is a tutorial on the Microsoft website for HUGO websites.**

![Image](images\ICT Helpdesk Migration\11.png "Image")

**The build was successful and deployed.**

![Image](images\ICT Helpdesk Migration\12.png "Image")

**The ICT Helpsite can be viewed at the new AZURE URL**

![Image](images\ICT Helpdesk Migration\13.png "Image")

###### March 11

... Meeting with Rob to discuss updating the contents