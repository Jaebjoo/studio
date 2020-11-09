---
title: Studio 5 Linux Configuration
layout: default
description: Studio 5 Linux Configuration
---

## Studio 5 : 
# Linux Configuration

#### Client's Requests

![Client Request](images\Linux_Configuration\0Linux Architecture.png "Client Request")

Client requests 3 VMs connected on 3 different networks. 2 VMs connected to 1 gateway VM, connected to the internet with a public IP.

#### Summary 

3 VMs were created with 3Vnets which were peered to one of the Vnets.
VM connectivity was successful, however seperate NIs, a total of 3 needed for the gateway VM was difficult to implement and very costly.
Next step would be to try and create a virtualised environment inside the VM itself that can recreate the architecture.
Azure has limitations which are not well suited to this particular request. Azure is streamlined for a mainstream, corporate demand for virtual cloud infrastructures.

#### Reflection

* I am much more comfortable with creating VMs and resizing them for a particular purpose. 
* Networking VMs as well as different Vnets to have successful connectivity will be useful skills later on when appproaching more sophisticated architecture.
* I am more aware of size restrictions, NI limitations of each VM size and also the corresponding costs which may be a large burden.
* Theoretically, bridging on the gateway vm after attaching the NI would be possible, though I believe realistically, simply peering Vnet2 to 3 would be a easier solution.
* I have become more aware of the use of a gateway VM which serves to limit public connection and security against outside threats.
* Azure Bash shell is very responsive and allows easy access to each VM
* Network security can be managed at each individual level with a firewall configured within the VM as well as in the Azure portal.
* Overall, it was a valuable experience to learn advanced features of VMs and Networking.


#### Solving Solution

**Creating VNets**

3 Vnets were created in total on Azure

![Vnet List](images\Linux_Configuration\1vnetList.png "Vnet List")

Vnet 1 was peered to Vnet 2 and 3

![Vnet 1 Peering](images\Linux_Configuration\2vnet1peering.png "Vnet 1 Peering")

Vnet 2 and 3 peered to 1

![Vnet 2 Peering](images\Linux_Configuration\3vnet2peering.png "Vnet 2 Peering")
![Vnet 3 Peering](images\Linux_Configuration\4vnet3peering.png "Vnet 3 Peering")

VMs added to each Network

![VM1 Network](images\Linux_Configuration\5vnet1.png "VM1 Network")
![VM2 Network](images\Linux_Configuration\6vnet2.png "VM2 Network")
![VM3 Network](images\Linux_Configuration\7vnet3.png "VM3 Network")

Complete architecture of the networks.

![Networks](images\Linux_Configuration\5-0vnetPeering.png "Networks")

VM1 has a public ip of 104.210.108.234.
Open bash shell on Azure and connect using this ip.

![VM1IP](images\Linux_Configuration\8vm1ip.png "VM1IP")

Type in the command below and enter the password

![VM1Connection](images\Linux_Configuration\9vm1connection.png "VM1Connection")

VM2 and 3 have not been given public IPs and can only be accessed through the gateway VM

![VM2Connection](images\Linux_Configuration\10vm2connection1.png "VM2Connection")

VM2 private IP

![VM2Connection](images\Linux_Configuration\11vm2connection2.png "VM2Connection")

VM3 private IP

![VM3Connection](images\Linux_Configuration\12vm3connection.png "VM3Connection")

Use these private IPs to ssh from VM1(gateway VM).

Pinging to test connections to both VMs using Private IP

![VM2 Ping](images\Linux_Configuration\13vm2ping.png "VM2 Ping")
![VM3 Ping](images\Linux_Configuration\14vm3ping.png "VM3 Ping")

ssh to VM2 using private ip

![VM2 SSH](images\Linux_Configuration\15vm2connection3.png "VM2 SSH")

VM1 also has a private VM, ping testing from VM2 to VM1 is successful, however you cannot ping from VM2 directly to VM3.
A simple peering from Vnet2 <> Vnet 3 would solve this issue, however the client requests a bridge be used on VM1 to have connection.

![VM1 Private IP](images\Linux_Configuration\16vm1privateip.png "VM1 Private IP")

![VM1 Ping Success](images\Linux_Configuration\17vm1ping.png "VM1 Ping Success")

![VM3 Ping Fail](images\Linux_Configuration\18vm3pingfail.png "VM3 Ping Fail")

With the network topology completed, additional NICs should be attached to complete the configurations.

NICs can be added in the Networking section of the "Settings"

![VM Networking](images\Linux_Configuration\19vmnetworking.png "VM Networking")

New Network interface can be created and attached to the VM

![VM NIC Diagram](images\Linux_Configuration\33vmnicdiagram.png "VM NIC Diagram")

![VM NIC](images\Linux_Configuration\20vmnic.png "VM NIC")

![VM NIC Attach](images\Linux_Configuration\21vmnicattach.png "VM NIC Attach")

![VM NIC Adding](images\Linux_Configuration\22nicadding.png "VM NIC Adding")

![VM NIC Attached](images\Linux_Configuration\23nicattached.png "VM NIC Attached")

However when a second network interface is added and attaching is attempted, it fails. Particular Azure VMs have a resstriction on the number of NI allowed. The maximum on the VMs on this try allowed only 2.

![VM NIC Adding Fail](images\Linux_Configuration\24nicadding2.png "VM NIC Adding Fail")

![VM NIC Adding Fail](images\Linux_Configuration\25nicaddingfail.png "VM NIC Adding Fail")

NI have their own individual public and private IPs.

![VM NIC IP](images\Linux_Configuration\26nic1ip.png "VM NIC IP")

![VM NIC IP](images\Linux_Configuration\27nic2ip.png "VM NIC IP")

These can be seen within the VM with the ' ip a ' command.

![VM NIC IPs](images\Linux_Configuration\28nicipinvm.png "VM NIC IP")

The size of a VM can be adjusted on the size section of settings

![VM Size](images\Linux_Configuration\29changingvmsize.png "VM Size")

https://github.com/uglide/azure-content/blob/master/articles/virtual-network/virtual-networks-multiple-nics.md

A github article about the VM sizes can be seen in the link above

A comprehensive list of the number of NIC that can be attached to each VM size is available here.

![VM NIC capacity](images\Linux_Configuration\34nictable.png "VM NIC capacity")

![VM Size](images\Linux_Configuration\29changingvmsize.png "VM Size")

![VM Size](images\Linux_Configuration\30changingvmsize2.png "VM Size")

There may be restrictions on the available VMs based on which region you have established your infrastructure. Costs are also a very significant factor when considering a size upgrade. The A4 which was the final solution to this problem costs +200 Dollars per month. 

This was a critical feasibility issue and a new solution had to be found.

However the A4 was able to have 3 different NIC as requested.

![VM New Size](images\Linux_Configuration\31nicnewsize.png "VM New Size")

