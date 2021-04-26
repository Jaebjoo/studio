---
title: Studio 6 
layout: default
description: Decommissioning OP Infrastructure
---

## Studio 6 : 
# Decommissioning OP Infrastructure

#### Client's Requests

Job assigned **April 12**

Due Date **April 29**

Job Completed **April 22**

As the OP infrastructure is being migrated to the Azure Cloud, physical devices need to be decommissioned.

Services on these devices have been audited and authorised to be shut off.
The devices will be shutdown and physically removed.

Access to the management interface of the devices needed to be determined

A screen was connected on the devices to see the terminal which displayed the following message.

![Image](images\Decommissioning\IMG-0733.jpg "Image")

**These were the 4 machines tha needed to be shutdown.**

**The NAS machines have the storage for the other 2 servers. NAS stands for Network attached storage.**

![Image](images\Decommissioning\IMG-0735.jpg "Image")

![Image](images\Decommissioning\IMG-0737.jpg "Image")

**The terminal could be accessed but the management had to be done from a web browser on that IP.**

![Image](images\Decommissioning\IMG-0738.jpg "Image")

![Image](images\Decommissioning\Screenshot 2021-04-22 135555.png "Image")

**Log In credentials were provided by Rob, This is the view of the log in screen on the web browser. The Username "Root" was obtained from the terminal screen.**

**Once we were successfully logged on, we stopped all the services that were running.**

![Image](images\Decommissioning\Screenshot 2021-04-22 135639.png "Image")

![Image](images\Decommissioning\Screenshot 2021-04-22 135934.png "Image")

![Image](images\Decommissioning\Screenshot 2021-04-22 141217.png "Image")

**Next were the NAS servers. The IP for the cloud1 server was 10.114.27.140, so Rob suggested we try IP addresses above and below that. We used a Nmap scan to see ports open on IPs below and Above .140 address. We were able to see port 80 open on 10.118.27.139**

![Image](images\Decommissioning\Screenshot 2021-04-22 141233.png "Image")

![Image](images\Decommissioning\Screenshot 2021-04-22 141342.png "Image")

![Image](images\Decommissioning\Screenshot 2021-04-22 141723.png "Image")

**We shutdown both 10.114.27.138 and .139 NAS Servers.**

![Image](images\Decommissioning\Screenshot 2021-04-22 143400.png "Image")

![Image](images\Decommissioning\Screenshot 2021-04-22 143414.png "Image")

**We then proceeded with shutting down the cloud01 .140 Server**

![Image](images\Decommissioning\Screenshot 2021-04-22 143523.png "Image")

![Image](images\Decommissioning\Screenshot 2021-04-22 143534.png "Image")

**We checked that the machines were shutdown upstairs in the server room. The power is still connected so it has an orange light. We couldn't view the terminal of Cloud2 and could not find any IPs serving on a port 80 for Cloud2 leading us to reach the conclusion that Cloud2 was offline to begin with.**

![Image](images\Decommissioning\unnamed.jpg "Image")

![Image](images\Decommissioning\unnamed1.jpg "Image")

**We confirmed that the Machines were shutdown and confirmed with Rob that he was happy with the job done before closing the ticket.**