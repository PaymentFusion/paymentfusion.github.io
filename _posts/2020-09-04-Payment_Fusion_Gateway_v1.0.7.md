---
layout: post
title: Payment Fusion Gateway v1.0.7
tag: Payment Fusion Gateway
author: AxiaMed
---

This release adds additional features the Loopback (Approve All) Processor Handler, resolves some issues in the reporting responses, includes UI updates in the portal, and improves the performance and stability of the gateway. 

#### Features
* The Loopback (Approve All) AuthorizedAmount is populated (echoed) from the transaction request.
* Added ResponseCode: 85 to Loopback processor.
* Common phone number formats may now be pasted into phone-number fields.


#### Bugs
* The gateway now honors the Partial Auth Support setting of the merchant unless it's explicitly overwritten.
* Fixes a reporting issue where the transaction's associated records were incorrect.
* Fixes an issue the prevented cash transactions from being returned in the reporting response.
* Batches that include captured transactions now settle properly.
* Partial auth indicated is now supported for AuthOnly and Refund transaction requests.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Tuesday, September 8 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Wednesday, September 9 between 5:00 PM and 6:00 PM Pacific.
