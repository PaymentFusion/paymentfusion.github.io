---
layout: post
title: Transaction Broker v1.53.0
tag: Transaction Broker
author: AxiaMed
---

This release improves customer engagement on the terminal and adds support for healthcare data with transactions. This release also makes improvements to the API documentation and fixes a number of other issues.

#### New features
* Transaction Broker will now identify HSA/FSA cards via the `is_healthcare` field. 
* Transaction Broker now supports a healthcare object (see below) for auto-substantiation of healthcare-related purchases (pending certification).
    * Polling and callback responses now include the healthcare object.
* Improves the success rate on transactions by automatically retrying the transaction when a "recoverable" error occurs.
* Android payment devices support formatted text in prompt jobs.
* Added an option to remove the "No" and "Cancel" buttons when sending a "yes/no" or "ok/cancel" prompt, respectively.
* Added an option to prevent the terminal from displaying the "Idle" screen when sending multiple prompt jobs.
* Transaction requests support up to 6 decimal places in the amount fields.
    * Note: Transaction Broker only supports US Currency. Numbers after the second decimal place must be zeros. e.g. `amount: "4.2500000"`  

###### Healthcare Object
```javascript
"healthcare": {
    "iias_verified": null,
    "healthcare_amount": "0.00",
    "prescription_amount": "0.00",
    "copay_amount": "0.00",
    "vision_amount": "0.00",
    "clinic_other_amount": "0.00",
    "dental_amount": "0.00",
    "transit_amount": "0.00",
    "cumulative_amount": "0.00"
}
```

#### Bug fixes
* Improved the handling of transaction requests when the gateway is unavailable.
* The `amount` and `auth_amount` in a refund / return transaction response will return the `refund_amount` of the request.
* URLs are now validated on the `POST /hpps` endpoint. 

#### Documentation updates
* `POST transactions/process/ach` endpoint has been updated to show the allowed values on `sec_code`.
* `POST transactions/refund/ach` endpoint has been updated to validate the `sec_code` property, since it is a required field.
    * Added the "required" indicator for `sec_code`.
* The documented status code for a successful response on `POST /prompt_jobs` has been changed to `201`.
* The `action_taken` field has been removed from the success response for the following endpoints:
  * `POST /transactions/process/{card/ach/cash}`
  * `POST /transactions/refund/{ach/cash}`
* Missing error codes have been added to the following endpoints:
  * `POST /hpps` → 85, 106
  * `POST /prompt_jobs` → 85, 106
  * `POST /print_jobs` → 124, 127, 130, 132, 133, 134, 135, 137, 139, 140, 141, 143, 149, 150, 153, 159, 160, 161
  * `POST /transactions` → 164, 166, 167, 168, 257
  * `POST /transactions/refund/card` → 58, 200
  * `POST /transactions/process/ach` → 198, 202, 206
  * `POST /transactions/process/card` → 205 , 219, 227, 228, 229
  * `POST /transactions/process/cash` → 201, 229
* `POST /promt_jobs` has been updated to reflect that `message` is not required when `type: "signature"`.
* Documentation for `client_id` and `serial_number` has been updated to correctly indicate that one, or the other, is a required value.
* `amount` is now correctly identified as a "string" in `POST /transactions/process/ach`.
* Callback request schema has been added to the `POST /transactions/refund/ach` endpoint
* **Example Value** has been added to a number of endpoints. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, May 6 between 12:00 AM and 1:00 AM PDT
<br>
**Production**: Thursday, May 7 between 12:00 AM and 1:00 AM PDT
