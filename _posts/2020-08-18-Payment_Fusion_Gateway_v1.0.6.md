---
layout: post
title: Payment Fusion Gateway v1.0.6
tag: Payment Fusion Gateway
author: AxiaMed
---

This release supports overriding partial authorization settings on the merchant, adds reporting data, includes UI updates in the portal, and improves performance and stability of the gateway. 

#### Features
* Override partial authorization support on the merchant.
    * Support override for card-present and card-not-present transactions.
    * Adds an indicator when the processor approves a partial amount for a transaction.
* The gateway portal limits time zones to the United States.
* `source_type` and `source_name` are included in the transaction response.


#### Bugs
* Fixes an issue that could allow a cardholder to submit the HPP form multiptle times.
* Credit transactions with PIN are no longer recorded as debit.
* Correctly displays CareCredit in the transaction details on the portal. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Tuesday, August 11 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Thursday, August 13 between 5:00 PM and 6:00 PM Pacific.
