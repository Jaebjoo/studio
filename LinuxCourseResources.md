---
title: Studio 6 
layout: default
description: Linux Course Resources
---

## Studio 6 : 
# Linux Course Resources

#### Client's Requests

Job assigned **March 11**

Due Date **April 9**

Job Completed **March 29th**

![Image](images\LinuxCourseResources\Screenshot 2021-03-26 212002.png "Image")

Faisal has requested alternative teaching resources to teach his Linux Course as the necessary VM resources are unable to be created using Vsphere or VMWare as those licenses are due to expire and the OP infrastructure is being migrated to the cloud.

We have suggested a Docker Container Networking solution.

#### Summary

*(Docker conatiner network diagram)

**The feasibility of docker containers to replace the VMs required for the Linux Course Labs is a success. Bridging of multiple ethernet adaptors in a gateway container is successful using bridge utils.**

**We will proceed with scripting to automate the resource creation as well as Azure Lab services or DevTestLabs**

**We will also proceed with rewriting the Linux Course Labs 11-15**

#### Reflection

#### Worklog

###### March 18th

**This is the first attempt at creating a docker network.**
**There is a bridge called linux_bridge with two containers named LinuxPaper and LinuxPaper2**

![Image](images\LinuxCourseResources\Screenshot 2021-03-18 151055.png "Image")

**This is a summary of the container ip addresses in the docker bridge network.**

![Image](images\LinuxCourseResources\Screenshot 2021-03-18 152127.png "Image")

**This is a ping test from one container to another**

![Image](images\LinuxCourseResources\Screenshot 2021-03-18 152325.png "Image")

**This is a ping test from the host to the container**

![Image](images\LinuxCourseResources\Screenshot 2021-03-18 152619.png "Image")

**This is the details of the docker bridge network.**

**This bridge is visible from the host with ip addr show command.**

**From the host's perspective it is called br-c3288eeb762d**

![Image](images\LinuxCourseResources\Screenshot 2021-03-18 152717.png "Image")

**Pinging to the gateway is also capable from a container.**

![Image](images\LinuxCourseResources\Screenshot 2021-03-18 152847.png "Image")

###### March 27th

**There are now 3 containers. There are 3 networks. The gateway container is part of all 3 containers.**
**The other two containers are part of separate networks and connected to the gateway. The two isolated networks do not have masqerade enabled and do not have access to the internet by default through docker.**

**This is the route list on the gateway container**

![Image](images\LinuxCourseResources\Screenshot 2021-03-27 201159.png "Image")

**There was a loss of internet connection to the gateway even though the Gateway Network has masquerade function**

![Image](images\LinuxCourseResources\Screenshot 2021-03-27 201423.png "Image")

**ip route list shows that the deffault is via 172.30.0.1 which does not have masquerade function to outside internet**

**This must be changed with ip route add default via 192.168.32.1 dev eth 5**

**This will change the ip routing**

![Image](images\LinuxCourseResources\Screenshot 2021-03-27 203924.png "Image")

**A bridge was created with eth 8 and eth 9 connected to it. However iptables and forwarding has not yet been correctly configured to pass traffic from one isolated network to the other.**

###### March 29th

**Pinging from one network to the other is possible after changing the subnet of the containers.**

**Feasibility test is complete**

**DevOps team will now follow through with a rewrite of the Course Labs from 11 - 15 and also write scripts to automate the resource creation and explore Azure Lab services and DevTestLabs**

**We aim to create a comprehensive teaching resource for Faisal to use for his semester.**





#### Configurations

		//UPDATE THE VM

sudo apt-get update

	//INSTALL DOCKER
	
sudo apt install docker.io
sudo systemctl start docker
sudo systemctl enable docker

	//CREATE CONTAINER
	
docker run -i -t --name linuxPaper ubuntu /bin/bash
exit

	//START CONTAINER
	
docker start linuxPaper

	//STOP CONTAINER

docker container stop [container]

	//REMOVE CONTAINER

docker container rm [container]

	//SSH INTO CONTAINER

docker exec -it <container name> /bin/bash

	//CREATE NETWORK BRIDGE
	
docker network create -d bridge linux_bridge

docker network create \
--driver=bridge \
--opt com.docker.network.bridge.enable_ip_masquerade=false \
[bridge name]

--subnet=

	//SHOW DOCKER NETWORK LIST

docker network ls

	//REMOVE NETWORK BRIDGE

docker network rm [bridge]

	//INSPECT NETWORK BRIDGE
	
docker network inspect linux_bridge

	//CREATE CONTAINER TO NETWORK

docker run -d --net=linux_bridge --name linuxPaper ubuntu

	//CONNECT EXISTING RUNNING CONTAINER TO NETWORK

docker network connect linux_bridge linuxPaper

	//DISCONNECT CONTAINER FROM NETWORK

docker network disconnect [network] [container]

	// INSTALL UTILITIES IN CONTAINER
	
apt-get update
apt-get install iputils-ping
apt install iproute2
apt-get install vim
apt update -y
apt-get install iptables sudo -y

apt-get install bridge-utils
apt install net-tools

	//set up a user

adduser admin
adduser admin sudo

su - admin

	//start container with full permission

docker exec -it --privileged [container] /bin/bash

	//VM ip
	
ip addr show

GatewayVM
ens160: 10.25.137.151

	//docker container ip configurations

BatCave
Gateway: 172.23.0.1
ip: 172.23.0.2

docker0: 172.17.0.10
linux_bridge:172.19.0.4

WayneManor
Gateway: 172.24.0.1
ip: 172.24.0.2

docker0: 172.17.0.11
linux_bridge: 172.19.0.5

	//pinging from BatCave <> WayneManor not possible
	
	//bridging two NIC
	
http://www.microhowto.info/howto/bridge_traffic_between_two_or_more_ethernet_interfaces_on_linux.html
	
https://dzone.com/articles/step-by-step-guide-establishing-container-networki

https://www.thegeekstuff.com/2017/06/brctl-bridge/
https://help.ubuntu.com/community/NetworkConnectionBridge

ip addr flush dev [eth1]
ip addr flush dev [eth2]
brctl addbr [bridgename]
brctl addbr [bridgename] [eth1] [eth2]
ip link set dev [bridgename] up

brctl addbr
	//show bridges
brctl show
	//delete bridge
brctl delbr [bridgename]
	//add interface
brctl addif dev [interface]
	//add multiple interfaces
brctl addiff dev [interface] [interface]

{add ips to bridges}

	//ip commands

ip addr show
ip addr add [ipaddress] dev [eth]
(ip addr add 172.29.0.3/16 dev eth8)

ip addr del[ipaddress] dev [eth]
ip route show
ip link set [eth] up
ip link set [eth] down

ip route del default 
ip route add default via 192.168.32.1[gateway ip] dev [eth]


https://subscription.packtpub.com/book/networking_and_servers/9781785287916/1/ch01lvl1sec12/connecting-two-networks

http://ebtables.netfilter.org/br_fw_ia/br_fw_ia.html
