---
layout: post
title: Reporting API v1.9.0
tag: Reporting API
author: AxiaMed
---
The Reporting API is being updated to allow filtering by gateway, improve the consistency on amount fields, and resolve documentation issues and other bugs.

#### Features
* Search for, and sort records on the gateway where the transaction was performed.
* Some amount fields, such as `declines_amount`, `sales_amount`, `credits_amount`, etc., are represented as numbers, while others are strings. All amount-related fields will be represented as double-digit precision strings.

#### Documentation
* Error-response documentation has been improved.
* `source` has been deprecated and removed from the API documentation for search and sort fields.

> **Note**: The field is being removed from documentation only. Existing integrations will continue to work; however, transaction records from the legacy gateway via data-feed does not include source values. We will move to using the data-feed for legacy gateway starting April 1, 2020.
>
> ISVs should move away from searching by source to retrieve transaction records from the legacy gateway.

#### Other
* Improves monitoring of the Reporting API by employing a URL that returns the health of system and dependencies.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, March 11 between 1:00 AM and 2:00 AM PDT
<br>
**Production**: Thursday, March 12 between 1:00 AM and 2:00 AM PDT
