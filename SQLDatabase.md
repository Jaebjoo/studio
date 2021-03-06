---
title: Studio 6 
layout: default
description: SQL Database
---

## Studio 6 : 
# Create a SQL database

#### Azure Learn

https://docs.microsoft.com/en-us/learn/modules/azure-database-fundamentals/exercise-create-sql-database

Azure SQL Database is a relational database based on the latest stable version of the Microsoft SQL Server database engine. SQL Database is a high-performance, reliable, fully managed, and secure database. You can use it to build data-driven applications and websites in the programming language of your choice, without needing to manage infrastructure.

**Creating a SQL database as a PaaS will reduce administration costs and optimize activities. Backups, updates and other maintenance is fully managed.**

Creating this resource may be required for DB3.

**The following is the configurations for creating a SQL database PaaS**

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.29.14 PM.png "Image")

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.31.05 PM.png "Image")

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.32.11 PM.png "Image")

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.36.23 PM.png "Image")

**This is the overview page of the new SQL Server**

**Select Set server firewall, and then select Yes to Allow Azure services and resources to access this server**

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.37.31 PM.png "Image")

**Select the db1 entry representing the SQL database you created, and then select Query editor (preview) in the nav bar**

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.39.33 PM.png "Image")

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.39.48 PM.png "Image")

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.40.57 PM.png "Image")

**The connection with the IP address of the computer you are using is not allowed**

**This issue must be resolved by updating the firewall settings of the SQL DB**

**In Client IP address your IP will be shown. Select Rule name, add your IP in both the Start IP and End IP fields, and then select Save.**

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.41.20 PM.png "Image")

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.41.39 PM.png "Image")

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.41.44 PM.png "Image")

**After you sign in successfully, the query pane appears. Enter the following query into the editor pane**

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.52.24 PM.png "Image")

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.53.58 PM.png "Image")

**You can also see the sample data tables.**

![Image](images\Create SQL Database\Screen Shot 2021-01-18 at 8.54.09 PM.png "Image")