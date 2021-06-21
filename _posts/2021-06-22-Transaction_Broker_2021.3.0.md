---
layout: post
title: Transaction Broker 2021.3.0
tag: Transaction Broker
author: AxiaMed
---

This release improves the stability and reliability of Transaction Broker.

#### Features
* Support for upcoming terminal applciation diagnostic features.
* Passes the `description` field to the Payment Fusion Gateway on **POST** `/transactions/process/...`
* `remote_id` has been added to reversal / refund endpoints.
  *  **POST** `/transactions/reversal`
  *  **POST** `/transactions/refund/card`

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Moday, June 21 between 1:00 AM and 12:00 AM Pacific
<br>
**Production**: Tuesday, June 22 between 12:00 AM and 1:00 AM Pacific
