---
layout: post
title: Reporting API v1.11.0
tag: Reporting
author: AxiaMed
---
This Reporting API update improves the stability of the platform, and improves documentation. 

#### Features
* Control Center will generate UUIDs for an Organization's API ID.
  * This change applies for new integration partners only. Existing integrations will continue to use the current method for generating the API ID. 

#### Bugs
* Transaction reference data types are now consistent between the Reporting API and DB.

#### Documentation updates
* Add default behaviors for `start_date` and `end_date`.
* Added the default value for `match_all`.
* Improved the description for `sort`. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox:** Monday, May 18 between 12:00 AM and 1:00 AM PDT
<br>
**Production:** Tuesday, May 19 between 1:00 AM and 2:00 AM PDT
