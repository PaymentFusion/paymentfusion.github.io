---
layout: post
title: Control Center v2021.3.0
tag: Control Center
author: AxiaMed
---

This release enhances the user experience in Control Center and improves reporting.  

#### Features
* The `is_partial_auth` value has been added to reporting data set.
* The reporting directories have been renamed and updated to improve clarity.


#### Bugs
* Reporting: Fixes an issue where closed batches would not get synced correctly.
* Reporting: Resolves an issue to properly handle duplicate batch identifiers.
* Reporting: Fixes an issue that would incorrectly identify an indeterminate transaction.
* Reporting: Include `transaction_job_auth` and `transaction_credit` categories when calculating counts. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, March 1 between 12:30 AM and 1:30 AM Pacific.
<br>
**Production**: Wednesday, March 3 between 12:30 AM and 1:30 AM Pacific.
