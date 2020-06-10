---
layout: post
title: Payment Fusion Gateway v1.0.2
tag: Payment Fusion Gateway
author: AxiaMed
---

This release adds functionality for recurring payments, and improves stability and performance of the gateway. 

#### Features
* Create a recurring contract using data from Transaction Broker.
* Publish recurring transactions (a.k.a. installments) using the Transaction Response Queue (TRQ).
  * Transaction Broker will use the TRQ data to fulfill web hook requests.
* Create a token from ACH data.


#### Bug fixes
* Supports the `MerchantTransId` parameter via HPP for Elavon front-end. 
* Fixes an issue where Discover could be treated as a healthcare card.
* Improves reporting on healthcare data.
* `AuthorizedAmount` is populated with the refunded amount for a refund transaction.
* Fixes an issue where `IsHealthcare` could be returned `true`, even though the card that was used is not a healthcare card. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, June 8 between 5:00 PM and 6:00 PM Pacific.
<br>
**Production**: Tuesday, June 9 between 5:00 PM and 6:00 PM Pacific.
