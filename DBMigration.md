---
title: Studio 5 DB2/3 Migration
layout: default
description: Studio 5 DB2/3 Migration
---

## Studio 5 : 
# DB2/3 Migration

#### Client's Requests

![Client Request](images\DB_Migration\1ClientRequest.png "Client Request")

Client Requested the on-site teaching resources for DB2 and DB3 classes to be migrated to the Azure Cloud infrastructure.

The Azure solutions are to be researched and possible solutions accounting for features and costs are to be recommended

#### Summary

The focal point of the solution was the DBaaS vs IaaS
The current configuration of the resources are 2 VMs, one running MariaDB and one running a Docker service with SSMS server.

A simple lift and shift option would require two similar sized VMs to be created on the Azure infrastructure with adequate security configurations and automated tasks.

Research into the DBaaS solution revealed advantages of automated maintenance of the resources traded for the loss of custom scripts being able to be managed on the machines.

Costs were revealed to be similar for MariaDB solutions, though the SQL Server solution would be significantly different.

As the Microsoft solutions are tailored for corporate solutions which are heavy duty, they are resource heavy and consequently most costly than a single VM solution. Microsoft does not tailor for smaller operations.

Though Serverless single database solutions exist, which are charged on a transaction basis, it cannot handle multiple databases interlinked in a pool.

DB2 - MariaDB (DBaaS) Solution was chosen. A working prototype needs to be set up with users added.

DB3 - SQL Server needs to be created, although the DBaaS solution is being reviewed to determine whether costs are within budget.

#### Reflection

Through this task, I have learnt how to create VMs that are running MariaDB.
I have run scripts on these machines to add users.

I have also explored the DBaaS by creating a MariaDB Server.
A method of adding users to this server with a script and csv file is being reviewed.

This task gave me an opportnity to fully explore the Database solutions on Microsoft Azure.

I would like to explore the security features further next semester as well as user access methods and authority/permissions.

#### Findings and Solution

DBaaS has resources managed automatically by Azure such as patching, backups and restores if needed. There is no need to manage the VM.

The trade off is that custom made scripts are not easily able to be loaded onto a VM as there is no access to it.

Costs have been fully explored and have been determined to be similar. However the DBaaS offers a period reserved price for a discounted cost.

![DBaaS](images\DB_Migration\3DBaaSDiagram.png "DBaaS")

A short summary report was created comparing the two solutions.

More detailed documentation should be created in the future, however the report was positively received by Rob.

![DB Report](images\DB_Migration\2DBReport.png "DB Report")