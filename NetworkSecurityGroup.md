---
title: Studio 6 
layout: default
description: Network Security Group
---

## Studio 6 : 
# Configure network access to a VM by using a network security group

#### Azure Learn

https://docs.microsoft.com/en-us/learn/modules/secure-network-connectivity-azure/6-configure-access-network-security-group

**You can manage the connection to the VM using Network security groups to allow particular traffic.**

This can include SSH, HTTP, HTTPS.

This skill is essential for managing the network on Azure.

Configuring the Network security group is key to security on Azure.

**From Cloud Shell, run the following az vm create command to create a Linux VM**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.03.53 PM.png "Image")

![Image](images\NSG\Screen Shot 2021-01-21 at 8.05.18 PM.png "Image")

**Run the following az vm extension set command to configure Nginx on your VM**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.05.35 PM.png "Image")

![Image](images\NSG\Screen Shot 2021-01-21 at 8.07.05 PM.png "Image")

**Run the following az vm list-ip-addresses command to get your VM's IP address and store the result as a Bash variable**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.07.45 PM.png "Image")

![Image](images\NSG\Screen Shot 2021-01-21 at 8.08.23 PM.png "Image")

**Run the following curl command to download the home page**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.08.36 PM.png "Image")

![Image](images\NSG\Screen Shot 2021-01-21 at 8.09.07 PM.png "Image")

**You can see that the VM cannot be reached on port 80**

**Run the following az network nsg list command to list the network security groups that are associated with your VM**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.10.12 PM.png "Image")

**The output will be my-vmNSG, which the VM is on**

**Run the following az network nsg rule list command to list the rules associated with the NSG named my-vmNSG**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.10.41 PM.png "Image")

![Image](images\NSG\Screen Shot 2021-01-21 at 8.11.21 PM.png "Image")

**Only port 22 has been allowed for SSH, there is no Port 80**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.11.34 PM.png "Image")

**Run the following az network nsg rule create command to create a rule called allow-http that allows inbound access on port 80**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.11.52 PM.png "Image")

**To verify the configuration, run az network nsg rule list to see the updated list of rules.**

**The Port 80 has been added to the ports allowed**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.12.16 PM.png "Image")

**Run the same curl command that you ran earlier**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.13.40 PM.png "Image")

**This will return the content of the website.**

**You can also use the browser to confirm connection through port 80**

![Image](images\NSG\Screen Shot 2021-01-21 at 8.13.46 PM.png "Image")