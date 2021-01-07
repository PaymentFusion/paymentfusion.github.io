---
layout: post
title: Payment Fusion Gateway v2021.1.0
tag: Payment Fusion Gateway
author: AxiaMed
---

This release includes certification changes required for Apple Pay on the web, and delivers other usability features and bug fixes.

#### Features
* The gateway is now paginating the results from the `GET /merchant/{merchantKey}/contracts` API endpoint.
* The `CustomerId` is now included in contract responses.

#### Bugs
* Recurring contracts can now be created Quarterly, and Bi-Annually.
* The HPP response now formats the amount as currency.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Thursday, January 07 between 5:00 PM and 6:00 AM Pacific.
<br>
**Production**: Monday, January 11 between 5:00 PM and 6:00 PM Pacific.
