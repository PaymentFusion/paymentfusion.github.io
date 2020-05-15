---
layout: post
title: Reporting API v1.10.0
tag: Reporting API
author: AxiaMed
---
The Reporting API endpoint is being updated to add check status response, improve error responses, and expand the date window for transactions results.

#### Features
* Returns status and tracking information on ACH (check) transactions in the response for `GET /transactions/{id}`
* Reporting API will return up to 90 days of data within the previous 365 days.
    * The `start_date` and `end_date` parameters on /search endpoints are optional.
    * The API returns transactions for the **24 hrs.** after the `start_date`, when it is the only value provided.
    * The API returns transactions for the **24 hrs.** before the `end_date`, when it is the only value provided.
    * The API returns transactions for the **24 hrs.** prior to the current date when omitting both values.

#### Bugs
* Resolves incorrect error codes in the API response:
* `GET /batches/{id}` returns 400 Invalid Id (used to return 500), when the id is missing 
* Calling `GET` on `/transactions/search` and `/batches/search` now returns 404 Invalid API (used to return 500). Integrators should use **POST**.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox:** Tuesday, March 24 between 2:00 AM and 3:00 AM PDT
<br>
**Production:** Wednesday, March 25 between 12:00 AM and 1:00 AM PDT
