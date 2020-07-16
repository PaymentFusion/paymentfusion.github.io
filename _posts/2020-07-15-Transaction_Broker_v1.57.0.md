---
layout: post
title: Transaction Broker v1.57.0
tag: Transaction Broker
author: AxiaMed
---

This release enables mail-order / telephone-order (MOTO) workflows, and delivers performance and stability improvements.

#### New features
* MOTO Workflow
  * The transaction response now includes the order method. 
  * The transaction response now includes an indicator if the card is present for the transaction.
* Added `merchant_order_number` support for Chase reporting.
* A transaction will timeout after 5 minutes if not picked up by the terminal.
* Read transaction responses are available for 24 hours.

#### Bugs
* Removed a possible "race condition" when sending multiple transactions to a single terminal.
* Fixes an issue that would return the incorrect transaction read-response after sending a new transaction to a terminal if it power-cycled during a `confirm_amount` flow.

#### Documentation
* Removed create, update, delete endpoints for receipts.
* Added `gateway_identifier` to **POST** `/transactions/refund/card` response.
* Added the required indicator to `input_method` on **POST** '/print_jobs'.
* Added additional details to **POST** `/prompt_jobs` and **POST** `/receipt_jobs`

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, July 20 between 12:00 AM and 1:00 AM PDT
<br>
**Production**: Monday, July 27 between 12:00 AM and 1:00 AM PDT
