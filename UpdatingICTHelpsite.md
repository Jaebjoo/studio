---
title: Studio 6 
layout: default
description: Updating ICT Helpsite
---

## Studio 6 : 
# Updating ICT Helpsite

#### Client's Requests

Job assigned **March 11**

Due Date **March 25**

Job Completed **March 25** (updated)

Rob has requested the DevOps team to update the live website on fthictweb08.ict.op.ac.nz.

#### Summary

Although the ICT Helpsite has been migrated to a static web app on the Azure infrastructure, the live website is already out of date and needs to be updated. This involved removal of information which was out of date. 

Any new features and content will be added to a rebuilt ICT Helpsite serving on the Azure Static Web App. The work for the rebuild will be carried out during  2021 Semester 2, led by Isaac (DevOps Team)

The ICT Helpsite is stored in a folder on the server and being served using Microsoft Internet Information Services Manager.

We needed to find the files and edit the html files. The site was updated automatically as it is serving html files directly without a separate build.

#### Reflection

The site was poorly designed with very limited knowledge of Web Development. Every file was named index.html and there was no modular design. There was a lot of copy and pasting and repetitive code. Though it has been temporarily updated there is a lot of potential for the rebuilt website.

There was very good team chemistry between Isaac, Rohill and I and I look forward to working productively together for the remaining 10 weeks of the semester.

#### Worklog

###### March 25th

**The site was pulling html files from the following directory.**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 085314.png "Image")

**A Folder shortcut was created for members to conveniently find it.**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 085403.png "Image")

**Internet information services Manager is being used to serve the site. I believe it is similar to Apache which I have had experience using.**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 085448.png "Image")

**For every site being served there are management tools for adminstrators to manage the website. We were particularly interested in restarting and stopping the service to update the content. It was possible to browse the url and also easily view the page sources.**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 085612.png "Image")

**The sidebar lists the sites that are being served.**

**Although only 1 site is being served... strangely there are isolated links which direct users to the original site. E.G the https-vmware page is actually within the "help" site, as is the "afterHours" page.**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 085640.png "Image")

**The following is the index.html file which was editted to remove the unused links and out of date content.**

**Any new content will be rebuilt. It was difficult to find the right page as all the pages are named "index.html**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 085901.png "Image")

**The site is organised into pages and posts.**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 090123.png "Image")

**These are the pages**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 090147.png "Image")

**These are the posts, which are also viewed as pages and also repeated (hardcoded) on the index page.**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-24 090205.png "Image")

**The following is a REBUILD PROPOSAL for the second semester Studio 5 students to work on to rebuild the entire site to be served on Azure Static Web App.**

**This proposal includes an overall purpose of the website and also the features/content to be included to fulfil this purpose.**

**Isaac will be leading/overseeing this project which will increase the presence/relevance of the DevOps team within the BIT department.**

![Image](images\ICThelpsite Screenshots\Screenshot 2021-03-29 161004.png "Image")
