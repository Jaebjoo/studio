---
title: Studio 6 
layout: default
description: Puppet X Docker
---

## Studio 6 : 
# Puppet X Docker

#### Research

https://forge.puppet.com/modules/puppetlabs/docker

![Image](images\puppetXdocker\Screenshot 2021-04-26 153124.png "Image")

DevOps team needs to solve a solution for the SysAdmin paper which needs 4 VMs running puppet, 1 puppet server and 3 agents.

We are researching the feasibility of running puppet on docker containers.

Puppet in docker would not only make the puppet infrastructure highly portable, it would reduce the need for multiple VMs and have 1 VM instead.

We are aware that the 1 VM needs to have sufficient performance requirements to be able to run 4 different services.

It would also be a challenge to run the 4 docker containers to simulate the operations week.

Docker Hub has puppet host and agent images. We have written a proposal to pursue this solution.

At the moment it seems possible that we have 4 different containers running on a docker network, communicating with each other.

We must consider that the App server be able to serve to a designated port on the host VM and also direct the traffic within the network to allow storage in the DB container. The DB container also needs to have sufficient storage space to be able to run the operations assignment.

![Image](images\puppetXdocker\Screenshot 2021-04-26 152643.png "Image")