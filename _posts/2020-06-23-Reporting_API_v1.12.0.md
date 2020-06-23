---
layout: post
title: Reporting API v1.12.0
tag: Reporting API
author: AxiaMed
---
This Reporting API update adds healthcare fields, identifies recurring transactions, and delivers stability and performance updates. 

#### Features
* Adds healthcare fields to transaction records.
  * is_healthcare: boolean
  * iias_verified: text
  * healthcare_amount: decimal
  * prescription_amount: decimal
  * copay_amount: decimal
  * vision_amount: decimal
  * clinic_other_amount: decimal
  * dental_amount: decimal
  * transit_amount: decimal
  * cumulative_amount: decimal
* Adds recurring fields to transaction records.
  * is_installment: boolean
  * customer_id: string
* Added transaction filters `is_recurring` and `customer_id` via Reporting API.


&nbsp;  
###### Deployment schedule
* * *
**Sandbox:** Wednesday, June 24 between 1:00 AM and 2:00 AM PDT
<br>
**Production:** Thursday, June 25 between 12:00 AM and 1:00 AM PDT
