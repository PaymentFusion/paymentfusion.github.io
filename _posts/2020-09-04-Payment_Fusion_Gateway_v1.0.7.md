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
* Loopback (Approve All) now includes Debit option.
* Common phone number formats may now be pasted into phone-number field when creating a TSYS merchant.
* Added logic to handle the `iias_verified` parameter for non-Mastercard card brands.



#### Bugs
* The gateway now honors the Partial Auth configuration of the merchant, unless it's explicitly overwritten by the integrator.
* Fixes a reporting issue where the transaction's associated records were incorrect.
* Resolves a situation that prevented cash transactions from being included in the reporting response.
* Fixes an issue that included the wrong associated transactions in a refund record.
* Batches that include captured transactions now settle properly.
* Partial auth indicated is now supported for AuthOnly and Refund transaction requests.
* Settlement reports now show Auth → Capture transactions.
* Fixes an issue that displayed an incorrect amount for a partial authorization on an Auth-Only transaction.
* Adds Loopback properties that were missing in Loopback (Approve All).
* Removes trailing zeros from EMV data in the response queue.
* Fixes an issue where the partial auth setting for Healthcare, MOTO Healthcare, and MOTO is not honored.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, September 14 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Tuesday, September 15 between 5:00 PM and 6:00 PM Pacific.
