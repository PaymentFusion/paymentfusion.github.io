---
layout: post
title: Payment Fusion Gateway v2021.3.0
tag: Payment Fusion Gateway
author: AxiaMed
---

This release provides fixes for DST time change, and delivers other usability features and bug fixes.

#### Features
* An `ActivationStatus` parameter has been added to the "Contracts" endpoint that returns the current state of a contract.

#### Bugs
* The Auto Close Time will no longer change on the merchant after Daylight Savings / Standard time changes.
  * The batch auto-close time will remain consistent and close at the expected time.  
* Adds validation for special characters and value length in address fields.
* The `TotalRecordCount` in the "Contracts" response now displays the correct number of records when setting the page value larger than the number of pages in the result. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, March 10 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Friday, March 12 between 5:00 PM and 6:00 PM Pacific.

