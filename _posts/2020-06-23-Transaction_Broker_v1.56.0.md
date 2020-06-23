---
layout: post
title: Transaction Broker v1.56.0
tag: Transaction Broker
author: AxiaMed
---

This release extends support for recurring transactions to payment devices running PFTA—Android, and delivers performance and stability improvements.

#### New features
* Recurring parameters in **POST** `/transactions` are supported regardless of payment hardware.
  * Provides parity between payment devices running PFTA—Telium and PFTA—Android.
  * The response includes a reference to the recurring contract as `customer_id`.
* Includes ACH tokens in the polling and web hook response on POST `/transactions/process/ach`.

#### Documentation updates
* The documentation for recurring parameters has been updated to reflect support on PFTA—Android.
* Fixed the description for `transactions/refund/(ach | cash | card)`.
* Added a description for `/hpps` and `scan_code` endpoints.
  * Added a description for `ammount` on the `scan_code` endpoint.
* Updates the `/transactions` response to match the current behavior.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Thursday, June 18 between 4:30 AM and 5:30 AM PDT
<br>
**Production**: Wednesday, June 24 between 12:00 AM and 1:00 AM PDT
