---
layout: post
title: PFTA—Telium v1.80.0 / v1.81.0
tag: PFTA-Telium
author: AxiaMed
---
This release of Payment Fusion Terminal Application for Telium (PFTA—Telium) improves security and performance. 
#### Features
* The terminal application now connects to a new polling endpoint, which improves performance.
* Card-brand standards for CVM limits have been aligned across processors.
* Authentication token expiry may now be adjusted by Payment Fusion.
  
#### Bugs
* Restores the terminal alert when an EMV card remains inserted after the transaction is complete.
* Fixes an issue where the terminal would not prompt for a PIN when the EMV card's preferred CVM is PIN.

&nbsp;  
###### Deployment schedule
* * *
**PFTA—Telium v1.80.0** is available now in all environments for TSYS and First Data merchants.
<br>
**PFTA—Telium v1.81.0** is available now in all environments for Chase merchants.
