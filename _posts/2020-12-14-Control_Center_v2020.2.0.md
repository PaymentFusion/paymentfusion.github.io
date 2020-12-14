---
layout: post
title: Control Center v2020.2.0
tag: Control Center
author: AxiaMed
---

This release enhances the user experience in Control Center and improves reporting.  

#### Features
* AxiaMed Admins and Support users may add an internal ID on an Organization.
* The EMV setting now defaults to "true" when creating a new merchant.
* Improved "Handshake" support in reporting.


#### Bugs
* Fixes an issue where the number of terminals reported on the dashboard, and the count of terminals in the terminal menu were out of sync.
* Resolves an issue where the "Save Changes" button would not be disabled.
* Reporting: The `batch_id` is now updated for authorize → capture transaction flows.
* Reporting: Tip amount has been added to the API response.
* Reporting: Fixes an issue that prevented valid source credentials from being synced.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, December 16 between 12:00 AM and 1:00 AM Pacific.
<br>
**Production**: Monday, December 21 between 12:00 AM and 1:00 AM Pacific.
