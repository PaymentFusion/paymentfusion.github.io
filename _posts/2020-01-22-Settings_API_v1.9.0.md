---
layout: post
title: Settings API v1.9.0
tag: Settings API
author: AxiaMed
---
The Settings API is being updated to enabled terminals run production transactions without EMV Certifications, improves error responses, and resolves issues.

#### Features
* Terminals may now use the “Force MSR” option in Control Center to prompt cardholders to swipe their cards when processing transactions in environments awaiting EMV Certification.
* Introduces new API responses for `accept header` errors:
  * The accept header is missing.
  * The accept header does not have the correct format.
  * The accept header version is not valid.
  * The request is not valid. Check URL or HTTP verb.


#### Documentation
* Improves the accuracy of documentation by making it easier to catch errors when it is updated.
* Our build system now requires API Documentation to be generated.


#### Bugs
* Resolves an issue where Settings API logs were not being filtered correctly.
* Fixes an issue that prevented Settings API logs from being displayed on DataDog.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, January 27 between 1:00 AM and 2:00 AM PST.
<br>
**Production**: Tuesday, January 28 between 1:00 AM and 2:00 AM PST.
