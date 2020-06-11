---
layout: post
title: Transaction Broker v1.55.0
tag: Transaction Broker
author: AxiaMed
---

This release adds features and improves support for healthcare data.

#### New features
* Supports healthcare transactions for card-not-present transactions.
  * The healthcare object is now available on **POST** `/transactions/process/card`.
* Read transaction response now includes healthcare data.
* `is_healthcare` is set to false for transactions using payment devices running PFTA—Telium, or via USAePay gateway.
  * Support for the healthcare vertical is not available on USAePay.
* Programmatically cancel prompt jobs.
  * New endpoint: **PUT** `/prompt_jobs/{id}/cancel` 

#### Bug fixes
* Healthcare fields are no longer being passed unless explicitly set.

#### Documentation updates
* The documentation for Cumulative Amount, in the healthcare object, has been improved.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, June 15 between 12:00 AM and 1:00 AM PDT
<br>
**Production**: Tuesday, June 16 between 12:00 AM and 1:00 AM PDT
