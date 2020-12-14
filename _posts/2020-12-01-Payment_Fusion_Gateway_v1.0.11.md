---
layout: post
title: Payment Fusion Gateway v1.0.11
tag: Payment Fusion Gateway
author: AxiaMed
---

This release prepares the gateway for Apple Pay on web features, and delivers a number of bug fixes. 

#### Features
* Apple Pay on Hosted Payment Page is testable via ISV Mock interface.
  * **Note**: Certification for Apple Pay via the web has not been completed. 

#### Bugs
* Fixes an issue that omitted the SEC codes from the Virtual Terminal when processing checks.
* The gateway now properly formats FSA amounts for First Data.
* Resolves an issue where Reversals on First Data would provide an incorrect POS Condition Code.
* Reporting API responses on ACH transactions have been normalized.
* Voiding a credit card transaction no longer returns check details.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, December 14 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Tuesday, December 15 between 5:00 PM and 6:00 PM Pacific.
