---
layout: post
title: Payment Fusion Gateway v1.0.9
tag: Payment Fusion Gateway
author: AxiaMed
---

This release improves the handling of reversals, voids, and refunds responses in transaction and batch report API responses. 

#### Bugs
* Fixes an issue where multiple Reversals amounts were cumulative. Subsequent reversal amounts now replace earlier ones.
* The transaction reporting API summary now include Void on Refunds in Total Amount and Void Amount calculations.
* The gateway now properly handles voids on credits in a settlement report.
* Partial authorizations now show the authorized amount in the Settlement interface.
* Fixes an issue where the Settlement interface would show a partial reversal amount, instead of the authorized amount.
* Resolves an issue where the "Manual Transaction" indicator is always checked.
* Fixes an issue to include PRA Reversals in the Settlement interface.
* Offline credit reversals are no longer sent to the processor.
* Partial PRA reversals are no longer being sent to TSYS with the wrong trans-code.
* The TSYS Processor Handler now supports the IIAS Verified "exempt" state.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, November 4 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Thursday, November 5 between 5:00 PM and 6:00 PM Pacific.
