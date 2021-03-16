---
title: Studio 6 
layout: default
description: Azure Fundamentals 5
---

## Studio 6 : 
# Azure Fundamentals 5 - Governance, Privacy and Compliance

#### Azure Research

https://docs.microsoft.com/en-us/learn/paths/az-900-describe-identity-governance-privacy-compliance-features/

These concepts were beyond the scope of the DevOps team and fell under the controls of Rob or Faisal.

However we needed a better understanding of Active Directory as this would provide student details which would be linked with automation of the distribution and allocation of resources to individual students who take particular courses and require certain resources for those courses.

Cloud Administrators can also restrict where resources can be created and also which can be created.

These would be concerns for administration.
Most of the time in the DevOps team we have been concerned with feasibility of solutions and implementing them. However I am aware that these governance and policy issues need to be established and adhered to in a professsional environment.

## Access Management

### Authentication and Authorisation

Authentication is establishing identity of the person or service accessing the resource.

Authorisation is establishing what level of access an authenticated person or service has to the resource.

### Azure AD (Active Directory)

Azure AD provides

Authentication - verifying identity, multi factor authentication, custom list of banned
passwords.

Single Sign On - Enables one username and password to access multiple applications
Application Management -

Device Management - registration of devices and restrict attempts to only those
coming from known devices.

## Multifactor authentication

3 categories,

Something the user knows - like email or password
Something the user has - like a code to a. Mobile phone
Something the user is - face, fingerprint scan on mobile phone devices

## Conditional Access

Complying with Industry standards of governance such as PCI DSS
Corporate or organisational standards such as ensuring network data is encrypted.

## Governance

Teams working on the Cloud have ability to create new resources whenever they need in order to work Agile, but they must be controlled with restrictions in place to increase governance

* Define strategy >> define why you’re moving to the cloud >> Document business outcomes >> Validate that migrating to cloud will give right return on investment

* Plan >> Digital estate - create an inventory of resources to migrate >> Allocate tasks to right people >> create plan to develop skills for individuals to operate in the cloud >> build comprehensive plan regarding development, operations, and business teams with shared cloud adoption goal

* Ready >> Create a landing zone for users to become familiar with tools >> Subscriptions with governance, accounting and security capabilities >> refine landing zone to meet needs

* Adopt >> Migrate and deploy first project >> Explore more complex migration scenarios

* Innovate >> Verify new investments in new innovations add value to business >> Check in frequently with customers to verify that you’re building what they need

## Govern

### Manage

### Azure Governance Strategy

* Billing - billing report per subscription . Chargeback of cloud costs and organise the
subscriptions by department or by project

* Access Control - subscription is a deployment boundary for azure resources. You can
control access to each subscription and isolate their resources from one another

* Subscription Limits - Subscriptions have limits for resources and number of resources
deployed.

### Roles

#### Owner / Reader / Contributor

* Resource Locks to prevent accidental deletion or changes
CanNotDelete - Cannot delete before removing the lock first
ReadOnly - Cannot delete or change the resource

* Azure Blueprints can prevent resource locks from being removed that must exist.

### Policy Definition

Allowed VM SKU
Allowed Locations
MFA - Multifactor authentication enabled.

![Image](images\AF5\Screenshot 2021-03-16 225852.png "Image")

Compliance and Government Regulations
Legal Information