---
title: Studio 5 System Audit
layout: default
description: Studio 5 System Audit
---

## Studio 5 : 
# System Audit

#### Client's Request

![Client Request](images\System_Audit\1AuditTicket.png "Client Request")

Client requests a audit of the servers on the 3rd floor of the BIT building.
The 2 servers in question are 

**bitpcloud01.staging.op-bit.nz**
**bitpcloud02.staging.op-bit.nz**

as well as the websites which are hosted on the gateway server.

Client wishes to turn off all unused VM's upon confirmation with owners.

#### Summary

The team had receive a password kept by the client to access the Servers. The servers could not be connected to on the physical interface as the screen was damaged. The servers could be accessed on the IPs 10.118.27.141.

A list of the VMs which were running was compiled in an excel file. 
The list of VMs were posted to all lecturers as we did not have a clear record of the owners of the VMs.
We had to await confirmation from the lecturers to confirm which VM's they owned and which could be shutdown.
The Excel file was updated accordingly after each response.
Not all VM's were accounted for and although VMs were turned off after a round of reponses, some VM's still need further follow up.

This audit was prepared in preparation for the migration of the polytechnic infrastructure to the Azure Cloud Service.

#### Reflection

* The job was a good opportunity for me to actually see the physical machines and examine the contents inside.
* It was a good opportunity to communicate with multiple users of the servers and ensure that service was continued for desired VM's as well as reducing the resources being consumed by the organisation.
* Though accessing and navigating through the infrastructure will need to be reviewed again so it is done without any problems or confusion in the future.
* I have a better understanding of the resources that are being used in the background to support the BIT faculty.
* I hope to build on this insight in the next semester as we prepare for the migration onto the Azure Cloud Infrastructure.

#### Procedures

Initial investigation of to servers by connecting to the ip through the broswer revealed a list of VM's which were running.

![Machine List](images\System_Audit\2ServerMachineList.jpg "Machine List")

![Machine List 2](images\System_Audit\3ServerMachineList2.jpg "Machine List 2")

A excel file was created to compile the list of VMs

The team reached out to all lecturers and received mesages specifying which were to be kept and shutdown.

![Messages with Lecturers](images\System_Audit\4MessagesFromLecturers.png "Messages with Lecturers")

The compiled list was updated and further responses are being waited on

![Final List](images\System_Audit\5spreadsheet.png "Final List")