---
title: Studio 6 Bridging
layout: default
description: Studio 6 Bridging
---

## Studio 6 : 
# Bridging

#### Research Summary

![Image](images\Bridging\Screenshot 2021-03-29 153216.png "Image")

In our task we need have a Gateway VM(container) which has 3 ethernet adapters, 2 of which are 2 different isolated networks. We need to bridge the two ethernet adapters so that devices through one ethernet adapter can be connected to the other devices through the other ethernet adaptor

bridge-utils needs to be installed onto the Gateway VM(container for this to work)

An Ethernet bridge is a device for forwarding packets between two or more Ethernets so that they behave in most respects as if they were a single network. It could be a physical device, but it is also possible for a bridge to be implemented entirely in software. The Linux kernel has the ability to perform bridging by means of the bridge module.

(http://www.microhowto.info/howto/bridge_traffic_between_two_or_more_ethernet_interfaces_on_linux.html)

(https://www.thegeekstuff.com/2017/06/brctl-bridge/)

**Command: Install bridge utilities**

apt-get install bridge utils

**The following is a list of possible commands which can be viewed with brctl command**

![Image](images\Bridging\Screenshot 2021-03-29 153440.png "Image")


