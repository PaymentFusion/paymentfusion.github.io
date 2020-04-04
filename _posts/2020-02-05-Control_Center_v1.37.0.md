---
layout: post
title: Control Center v1.37.0
tag: Control Center
author: AxiaMed
---
Control Center is being updated to support terminal application updated in the Sandbox environment, improve reporting, and update features to use a new logging environment. This release also addresses a number of bugs.

#### Features
* Changing the estate for one or more Telium terminals in the Sandbox environment will now trigger terminal application updates.
* Ensures reporting accuracy for a merchant by alerting the user when entering a duplicate gateway identifier (GID) in Gateway Settings.
* Improves performance of Transaction Reports (Exago) by prompting the user to select an organization if they are logged in with an AxiaMed or ISV role.
* Fetching logs from Control Center now uses DataDog.


#### Bugs
* Email addresses are now properly saved when updating a user.
* Start and end dates are returned to the last 30 days after clicking the “Reset all” button in the reports view.
* Improves sync time and reduces `Invalid Merchant` errors after updating sources for a terminal.
* Resolves an issue that could expose sensitive data in logging.
* Resolves a syncing issue between Control Center and IngEstate that could cause a `503 Service Unavailable` error when updating a terminal.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, February 10 between 12:00AM and 1:00AM PST.
<br>
**Production**: Tuesday, February 11 between 12:00AM and 1:00AM PST.
