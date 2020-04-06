---
layout: post
title: Transaction Broker v1.49.0
tag: Transaction Broker
author: AxiaMed
---
Transaction Broker is being updated to improve the consistency of data between the legacy environment (terminals and gateway) and the Payment Fusion environment. This includes the normalization of data in the transaction response, via Transaction Read requests, and callback URLs. This release also addresses documentation and some bugs.

#### Features
* `gateway_result_code`, `gateway_result_message`, `gateway_result_text` are now being populated consistently between gateways.
* `return_card_data` now operates as expected. Explicitly setting this property to true will include card data in the response, setting it to false will omit that data. The default value is `false`.
* `save_card` now operates as expected. Explicitly setting this property to true will return a token, setting it to false not. The default value is `false`.
* The Webhooks response now includes the gateway that triggered the callback.


#### Other changes
* Decreases the number of callbacks—due to updated transaction information—by increasing the likelihood a terminal will make its finalize call before the Transaction Response Queue (TRQ) is triggered.
* `action_taken` has been removed from the API Documentation for `POST /transactions/refund/card`, since it does appear in the response.

#### Documentation
* `POST /transactions` now lists 201 as the response code
* Updated description for `GET /prompt_jobs/{id}`
* The description for Error 198 has be changed for clarity


#### Bug fixes
* `tax_amount` property is now being passed to the legacy gateway.
* `amount` may no longer be an empty / null string for the following endpoints:
  * `POST /transactions`
  * `POST /transactions/capture`
  * `POST /transactions/process/(card | ach | cash)`
  * `POST /transactions/{id}/set_amount`
* Fixes an issue for PFTA—Android where the transaction status returns “error” on successful tokenization using a “save” command.
* `credit_card_token` is now null when a transaction is declined.

&nbsp;  
Deployment schedule
* * *
**Sandbox** — Wednesday, February 12, 2020 between 12:00 AM and 1:00 AM PST.
<br>
**Production** — Thursday, February 13, 2020 between 12:00 AM and 1:00 AM PST.
