---
title: Studio 6 Docker Networking
layout: default
description: Studio 6 Docker Networking
---

## Studio 6 : 
# Docker Networking

#### Research Summary

DevOps member Rohill and I have conducted research into Docker networking of containers to offer a teaching resource solution for the Linux Course that Lecturer Faisal is teaching.

Docker is able to create a virtualised networking environment where individual containers are able to be connected with various networking methods.
One of these methods is BRIDGES.

Bridges are a way to connect stand alone containers.

The following documentation on Docker was used to get a general understanding of Docker Networking.

https://docs.docker.com/engine/tutorials/networkingcontainers/

![Image](images\DockerNetworking\Screenshot 2021-03-26 211448.png "Image")

**When containers are created, they are added to the docker0 bridge network by default.**
This can be disabled and a bridge created by the user can be used.
Docker containers must be running while added to the bridge to be seen.

The bridge details can be show with following command:

docker neworking inspect [bridge] 

This will display default gateway ip addresses and the ips for the containers that are attached to the bridge.

![Image](images\DockerNetworking\Screenshot 2021-03-26 211515.png "Image")

**Containers can be a part different networks like above.**
These are connected via Veths to the Linux host.
They can ping the default gateway veth as well as the linux host eth.

![Image](images\DockerNetworking\Screenshot 2021-03-26 211728.png "Image")

**It is not until the the containers are a part of the same network that they are able to ping each other.**
Docker containers can be a part of multiple networks and every instance that they are added to a new bridge, a virtual ethernet adaptor is added to the container. The veth is visible as a eth within the container.

After this research we were able to proceed with the container networking solution.
However we were aware that the linux course resource solution requires that a "gateway" container/vm be a part of 3 multiple networks.
Bridge utils must be used to bridge the eths of the remaining branch containers without the branch containers being on the same network.

We will write a proposal to proceed with a feasability test to create a demo environment. We will request a VM from Faisal to be able to test the possible configurations.