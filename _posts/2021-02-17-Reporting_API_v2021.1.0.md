---
layout: post
title: Reporting API v2021.1.0
tag: Reporting API
author: AxiaMed
---
This Reporting API update delivers stability and performance updates. 

#### Features
* Input method has been added to the transaction response. The response includes the method used to capture card data (swipe, dip, tap, etc.) from the terminal.

#### Bugs
* Fixes an issue that prevented some credits from being calculated in the transactions summary.
* Resolves an issue where non-terminal credits (e.g. credit via Virtual Terminal) was omitted from the transactions summary.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox:** Tuesday, Feb 16 between 12:00 AM and 1:00 AM PDT
<br>
**Production:** Thursday, Feb 18 between 12:00 AM and 1:00 AM PDT
