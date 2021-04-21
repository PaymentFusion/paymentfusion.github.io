---
layout: post
title: Payment Fusion Gateway v2021.6.0
tag: Payment Fusion Gateway
author: AxiaMed
---

This release improves the stability and performance of the gateway.

#### Bugs
* Fixes an issue that excluded AVS data from recurring transactions.  
* Resolves multiple issues on the Transaction Response Queue (TRQ)
  * BIN Data could be omitted from a transaction response
  * `Level3Amount` value is missing 
* Voiding a card-not-present transaction on FirstData will no longer decline with an error.
* Fixes an issue where card verify for American Express EMV would fail. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, April 21 between 5:00 PM and 6:00 PM Pacific.
<br>
**Production**: Thursday, April 22 between 5:00 PM and 6:00 PM Pacific.

