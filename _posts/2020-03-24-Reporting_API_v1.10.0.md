---
layout: post
title: Reporting API v1.10.0
tag: reporting
author: AxiaMed
---
The Reporting API endpoint is being updated to add check status response, improve error responses, and expand the date window for transactions results.

#### Features
* Returns status and tracking information on ACH (check) transactions in the response for `GET /transactions/{id}`
* `start_date` and `end_date` parameters on /search endpoints supports up to 90 days of data for the last 365 days
  * Response will default to a 24 hour window after the `start_date` or prior to the `end_date` if only one value is set
  * Response will default to a 24 hour window from the current date / time if neither value is set

#### Bugs
* Resolves incorrect error codes returned in the API response:
* `GET /batches/{id}` returns 400 Invalid Id (used to return 500), when the id is missing 
* Calling `GET` on `/transactions/search` and `/batches/search` now returns 404 Invalid API (used to return 500). Integrators should use **POST**.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox:** Tuesday, March 24 between 2:00 AM and 3:00 AM PDT
<br>
**Production:** Wednesday, March 25 between 12:00 AM and 1:00 AM PDT
