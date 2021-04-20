---
layout: post
title: Reporting API v2021.2.0
tag: Reporting API
author: AxiaMed
---
This Reporting API update delivers stability and performance updates. 

#### Features
* Transaction records now include a `partial_auth` flag (true / false) to indicate a partial authorization.
* The API response will now return an appropriate error if the JSON body does not match the schema.

#### Bugs
* Improves validation and error response when searching on `reference_number`.
* Resolves an issue where voided transactions could be omitted from the results.
* Fixes an issue where the `transactions_returned` count would not reflect the correct number of transactions.
 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox:** Thursday, April 15 between 12:00 AM and 1:00 AM PDT
<br>
**Production:** Monday, April 19 between 12:00 AM and 1:00 AM PDT
