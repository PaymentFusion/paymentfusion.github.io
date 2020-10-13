---
layout: post
title: Payment Fusion Gateway v1.0.8
tag: Payment Fusion Gateway
author: AxiaMed
---

This release resolves some issues with healthcare object validation, and improves reporting. 

#### Features
* Healthcare transactions must include a healthcare amount.
* Added validation for Healthcare amount, which must be less than or equal to Total Amount of a transaction.
* Audited the gateway logging for general security improvements.
* Added validation on `CopayAmount` and `TransitAmount` as they related to healthcare amount.
* Adds void information to the settlement response.
* Adds reversal information to the settlement response.



#### Bugs
* Properly handles transactions for Visa, where the healthcare object only contains a value for `IIAS_Verified`.
* `IIAS_Verified` now supports the `expempt` value on Staging.
* Long merchant names (25+ characters) are now tolerated in healthcare transactions.
* The Batch Net amount is now correct when performing a credit on a force-capture.
* Correctly sends Purchase Return Authorization (PRA) refunds to the processor.
* Fixes an issue where the source can be unspecified on a batch report.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Tuesday, October 13 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Wednesday, October 14 between 5:00 PM and 6:00 PM Pacific.
