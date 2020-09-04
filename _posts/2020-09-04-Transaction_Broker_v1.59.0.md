---
layout: post
title: Transaction Broker v1.59.0
tag: Transaction Broker
author: AxiaMed
---

This release provides consistent support for receipts across gateways, enhances partial authorization, and delivers stability and performance improvements.

#### New features
* New **GET** `/receipts` endpoint retrieves a receipt image (.png format) for a transaction. Similar to **GET** `/transactions/receipt/render`, but provides a more simple request / response.
* New features for partial authorizations include:
  * `allow_partial_auth` is echoed in the transaction polling response and callback
  * The polling response and callback includes an indicator if there was a partial approval of the transaction amount.
  * Added `allow_partial_auth` to HPP.


#### Bugs
* Fixes an issue where Transaction Broker would return "Invalid Card Token" during a processor outage.
* Transaction Broker will no longer respond with a transaction error or cancelled transaction when there is a gateway timout.

#### Documentation Updates
* Additional error codes have been added to **POST** `/scan_codes`.
* `approved_redirect` and `decline_redirect` now show the maximum allowed character length in **POST** `/scan_codes`.
* Improved the descriptions for recurring fields.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, September 2 between 12:00 AM and 1:00 AM PDT
<br>
**Production**: Thursday, September 3 between 12:00 AM and 1:00 AM PDT
