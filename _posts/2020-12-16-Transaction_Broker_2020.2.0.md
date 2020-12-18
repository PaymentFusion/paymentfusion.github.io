---
layout: post
title: Transaction Broker 2020.2.0
tag: Transaction Broker
author: AxiaMed
---

This release and improves handshake reporting and resolves a few bugs. 

**NOTE:** The versioning schema has been changed for our product releases. All product releases going forward will adopt a notation using the current year, release count, and hotfix. (e.g. 2020.1.0). This schema will provide release-cycle flexibility, and make it easier to interpret a product's release. 

#### New features
* Improved tracking of Transaction Broker "Handshakes".
* Improved error response for when performing a void or reversal on force-capture transactions.
  * **Note**: Payment Fusion Gateway only.

#### Bugs
* Fixes an issue where the tip amount would not be included in the **POST** `/transactions/adjust` response.
* Transaction reports for ACH refunds now includes `associated_ref_num`.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Thursday, December 17 between 2:00 AM and 3:00 AM PDT
<br>
**Production**: Tuesday, December 22 between 1:00 AM and 2:00 AM PDT
