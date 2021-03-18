---
layout: post
title: Transaction Broker 2021.2.0
tag: Transaction Broker
author: AxiaMed
---

This release adds Recurring Contract management, enhances support for partial authorizations, and improves stability. 

**NOTE:** The versioning schema has been changed for our product releases. All product releases going forward will adopt a notation using the current year, release count, and hotfix. (e.g. 2020.1.0). This schema will provide release-cycle flexibility, and make it easier to interpret a product's release. 

#### New features
* Endpoints for Recurring Contract management
    * Get all contracts for a merchant
    * Get the details of an existing contract
    * Update a contract's amount and its status (enabled / disabled)
    * Delete an existing contract
* Adds support for the `allow_partial_auth` parameter on Payment Fusion Gateway.
    * POST `/transactions`
    * POST `/transactions/process/card`

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Tuesday, March 16 between 12:00 AM and 1:00 AM Pacific
<br>
**Production**: Thursday, March 18 between 12:00 AM and 1:00 AM Pacific
