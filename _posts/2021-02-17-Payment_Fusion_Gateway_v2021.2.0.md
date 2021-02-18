---
layout: post
title: Payment Fusion Gateway v2021.2.0
tag: Payment Fusion Gateway
author: AxiaMed
---

This release includes features and fixes for Apple Pay and Google Pay on the web, and delivers other usability features and bug fixes.

#### Features
* Google Pay may now be configured as a payment method for merchants on the Hosted Payment Page (HPP).
* Google Pay option has been added to the HPP. 
* Recurring contracts support a "disabled" state when it's created.
* The gateway now prevents partial authorizations if they are not allowed for the merchant, or on a transaction.

#### Bugs
* Apple Pay is not available on HPP for save-only transaction types.
* Removes the HPP Apple Pay option for auth-only transactions.
* Fixes an issue that delayed the batch from appearing in the gateway portal.
* The gateway now includes a "suspended" status for recurring contracts.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Tuesday, February 23 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Wednesday, February 24 between 5:00 PM and 6:00 PM Pacific.
