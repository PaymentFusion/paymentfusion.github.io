---
layout: post
title: Transaction Broker v1.52.0
tag: Transaction Broker
author: AxiaMed
---

Transaction Broker is being updated to improve performance, stability, and resolve  inconsistencies in the API documentation.

#### Bug fixes
* Fixes an issue where the transaction type could be set to “Save Only” as part of a Confirm Amount workflow. Transaction Broker will now return an error when combining `um_command: 'save'` with `confirm_amount: true`. 

#### Documentation updates
* The `POST /transactions/adjust` endpoint has been updated to ensure consistency when used, and to promote proper use of adjustments. This endpoint will add the `new_tip` amount to the original amount of the transaction, which is returned as the `auth_amount` in the response. 
  * Existing integrations are not affected by these changes. With new integrations, adjusts should only be used to add a tip to a transaction. Adjusting the balance independent of tipping and negative adjustments should not be performed.
  * `original_amount` — This parameter is introduced as an alias of new_amount to better reflect the expected value. `new_amount` is still available on the endpoint.
* The description for the `command` parameter for `POST /transactions/process/ach` has been updated to reflect the allowed values. 
* The `receipt_ref_num` was incorrectly shown as required on `GET /transactions/receipt/render`. The required indicator has been removed.

#### Other
* Improves monitoring of the Transaction Broker API that checks the health status of additional endpoints.

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, March 18 between 1:00 AM and 2:00 AM PDT
<br>
**Production**: Thursday, March 19 between 1:00 AM and 2:00 AM PDT
