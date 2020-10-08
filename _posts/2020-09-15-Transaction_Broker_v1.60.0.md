---
layout: post
title: Transaction Broker v1.60.0
tag: Transaction Broker
author: AxiaMed
---

This release provides consistent support for receipts across gateways, enhances partial authorization, and delivers stability and performance improvements.

#### New features
* Transaction Broker now uses gateway v2 endpoints for processing transactions.
    * Transaction requests (sale, sale:adjust, save, authorize, credit)
    * Process Card, ACH, Cash
    * Adjustment
    * Capture
    * Refund
    * Reversal
    * Void
* Adds support for setting the recurring start date to the first and last day of the month.
* Transaction Broker now supports "Reversals" for "authorize" transactions on the Payment Fusion Gateway.
* Supports the Purchase Return Authorization (PRA) `"result_code": "85"`, and returns the transaction as "approved".
* New endpoint, **POST** `/print_receipts`, supports receipt printing across gateways.

#### Bugs
* Fixes an issue where a transaction can get stuck if the Wi-Fi connection is interrupted.

#### Documentation Updates
* Resolved inconsistencies between the documented and actual response on **GET** `/transactions`

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, October 12 between 12:00 AM and 1:00 AM PDT
<br>
**Production**: Monday, October 19 between 12:00 AM and 1:00 AM PDT
