---
layout: post
title: Transaction Broker v1.54.0
tag: Transaction Broker
author: AxiaMed
---

This release adds the option to generate a QR Code that will point to our hosted payment page (HPP) for online payments. Additionally, it extends healthcare data support for transactions that use a token and delivers performance and stability improvements.

#### New features
* Generate a QR Code for HPP.
    * New endpoint: **POST** `/scan_codes` returns a base64 encode .png image of a QR Code
    * Scanning the QR Code with a device (tablet, mobile phone, etc.) will direct the user to the Payment Fusion Gateway's HPP. 
* `MerchantTransId` has been added to **POST** `/hpps`

#### Bug fixes
* Adds error handling for failed `short_url` when generating a hosted payment page.
* Transaction Broker now tolerates long messages in a response from the processor.

#### Documentation updates
* Transaction requests require one of `client_id` or `serial_number`, not both.
* `message_markdown` has been added / updated on th "Prompt Job" endpoint. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Thursday, May 28 between 12:00 AM and 1:00 AM PDT
<br>
**Production**: TBD
