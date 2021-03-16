---
title: Studio 6 
layout: default
description: Azure Fundamentals 4
---

## Studio 6 : 
# Azure Fundamentals 4 - Security

#### Azure Research

https://docs.microsoft.com/en-us/learn/paths/az-900-describe-general-security-network-security-features/

Security was always an area of concern for Rob and other lecturers who would become the owners of the resources.

We have not looked into security in detail in the DevOps team, but this learning path provides a brief outline of the Security Centre, Sentinel, Key Vault and Network Security functions.

These tools are essential in protecting the Azure Infrastructure from external threats. 

## Security

## Azure Security Center

![Image](images\AF4\Screenshot 2021-03-16 224324.png "Image")

Provides visibility of security posture across all of your services.

Secure score is a measurement of an organisation’s security posture.

Just-in-Time VM access - allows traffic during specified time when admin requests or
approves.

Adaptive application controls - Detects when unauthorised applications are running on
VMs, monitored by machine learning.

Adaptive network hardening - monitors internet traffic patterns of VM and compares
with NSG network security group and makes recommendations.

File integrity Monitoring - Monitor changes made to important files and registry
settings, applications that might indicate a security attack.

## Azure Sentinel

Collect cloud data
Detect previously undetected threats with comprehensive analytics
Investigate threats with artificial intelligence
Respond to incidents rapidly with build in orchestration and automation of tasks

![Image](images\AF4\Screenshot 2021-03-16 224401.png "Image")

## Azure Key Vault

Manage Secrets - You can use Key Vaults to securely store tokens, passwords,
certificates, API keys, and other secrets.
Manage Encryption keys
Manage SSL/TLS certificates
Store secrets backed by hardware security modules

![Image](images\AF4\Screenshot 2021-03-16 224429.png "Image")

* The physical security layer is the first line of defense to
protect computing hardware in the datacenter.
* The identity and access layer controls access to
infrastructure and change control.
* The perimeter layer uses distributed denial of service
(DDoS) protection to filter large-scale attacks before they can
cause a denial of service for users.
* The network layer limits communication between
resources through segmentation and access controls.
* The compute layer secures access to virtual machines.
* The application layer helps ensure that applications are
secure and free of security vulnerabilities.
* The data layer controls access to business and customer
data that you need to protect.

### Protect Virtual Networks by using Azure Firewall

### Protect from DDoS Attacks using Azure DDoS Protection

### Filter Network Traffic using network security groups