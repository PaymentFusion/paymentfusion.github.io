---
layout: post
title: Control Center v1.42.0
tag: Control Center
author: AxiaMed
---

This update delivers improvements for reporting, terminal behavior, and stability improvements. 

#### Features
* Stores transaction times in UTC regardless of source.
  * All transaction records, which were imported before this change, will have their times converted to UTC.
* Restricts the terminal timeout setting to a minimum of 60s and a maximum 300s.
* Adds healthcare data to transaction records in reporting.

#### Bugs
* Resolves some issues that could prevent transaction records from syncing. 


&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, June 17 between 12:00 AM and 1:00 AM Pacific.
<br>
**Production**: Thursday, June 18 between 12:00 AM and 1:00 AM Pacific.
