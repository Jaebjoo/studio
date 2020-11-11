---
title: Studio 5 Azure Dev Test Labs
layout: default
description: Studio 5 Azure Dev Test Labs
---

## Studio 5 : 
# Azure Dev Test Labs

#### Research Summary

Azure Dev Test Labs provides a more controlled environment for setting up VMs.

VM configurations can be saved as "formulas" and replicated at will.

"Artifacts" are extensions deployed on VMs.
These can be pre-configured before VMs are deployed.

Resources also have the option to be "claimed" and "unclaimed" by users.

Autoshutdown policies can also be set for VMs. This can significantly reduce costs and waste of resources.

It is my personal belief that having preset VM configurations that can be easily created, claimed, unclaimed, shutdown and replicated creates a more dynamic environment where resources are only used On Demand.

These might be more suitable for entities that require a predetermined set of resources for a short term rather than fixing long term VMs. This may be preferable for developers and testers. DevTest labs also allows self managed Resources by developers in a contained environment that do need to wait approvals from IT Sysadmins, giving more independence while allowing easy management of costs.