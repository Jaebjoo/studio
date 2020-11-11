---
title: Studio 5 User Adding
layout: default
description: Studio 5 User Adding
---

## Studio 5 : 
# User Adding

#### Client's Requests

Client requests drills to be conducted on the DB2 and DB3 VM's to add users and create docker containers for each user.

#### Summary

Following documentation and updating it as the team was a challenge. Though it created good communication between the team to cross check how the procedures were meant to be carried out.
DB2 Users were created using a script with a csv file of student details.
DB3 Users were also created in the same manner with the addition of docker container creations.

Full functionality was confirmed after procedures were carried out.
The Machines were reverted back to a restore point for other members to carry out the exercise.

#### Reflection

* It was a good opporunity to be exposed to scripting and automating tasks such as user adding and container creation
* It was also a good experience to work together as a team to update documentation and manuals to carry out procedures.
* As each team member followed the documentation, it was a check to see whether the procedures written were clear and concise enough for others to follow.
* This gave a clear insight into the importance of documenting CLEAR instructions with detailed evidence.

#### Procedures

Login to server to load scripts and csv

![Server Login](images\DB_User_Adding\1serverlogin.jpg "Server Login")

Run an update before the scripts are run

![Server Update](images\DB_User_Adding\2serverupdate.jpg "Server Update")

Run scripts with csv file as argument

![Run Script](images\DB_User_Adding\3runscriptadduser.jpg "Run Script")

Checking the users have been added correctly

![Check](images\DB_User_Adding\4useraddcheck.jpg "Check")

Checking Maria DB login successful

![DB Login](images\DB_User_Adding\5usermariadblogin.jpg "DB Login")

Adding Users to DB3 Server

![User Add DB3](images\DB_User_Adding\6db3useradd.jpg "User Add DB3")

Checking Docker Groups

![Docker Check](images\DB_User_Adding\7dockergroupcheck.jpg "Docker Check")

Creating containers after logging into a user

![Container Create](images\DB_User_Adding\8userlogincheckcontainercreate.jpg "Container Create")

Checking that the containers have been made.

![Container Check](images\DB_User_Adding\9dockercontainercheck.jpg "Container Check")