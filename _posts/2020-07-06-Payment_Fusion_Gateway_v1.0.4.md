---
layout: post
title: Payment Fusion Gateway v1.0.4
tag: Payment Fusion Gateway
author: AxiaMed
---

This release adds functionality for recurring payments, includes support Mail-order / Telephone-order, and improves stability and performance of the gateway. 

#### Features
* Mail-order / Telephone-order (MOTO) features have been added to the gateway response.
* Save and Authorize transaction types can now create a recurring contract.
* `customerId` is returned via Transaction Response Queue (TRQ) when creating a contract.
* Bi-weekly and bi-monthly are now interpreted as "every-other" week and month, respectively.

#### Bugs
* Resolves an issue when performing a capture / adjust transaction on the loopback processor handler.
* `billing_zip` is no longer required to create recurring contract.
* Fixed an issue where the gateway would create a recurring contract using a card that was not approved.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, July 6 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Tuesday, July 7 between 5:00 PM and 6:00 PM Pacific.
