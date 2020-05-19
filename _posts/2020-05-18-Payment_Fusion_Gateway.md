---
layout: post
title: Payment Fusion Gateway — 2020.05.21
tag: Payment Fusion Gateway
author: AxiaMed
---

This update adds support for healthcare, by adding data fields, enhanced IIN lookup, and transaction responses with healthcare data. 

#### Features
* The IIN lookup has been enhanced to identify healthcare FSA / HSA cards, and will return `is_healthcare: true` when it finds a match.
* The gateway now supports the full healthcare object, which was introduced in [Transaction Broker v1.53.0]({% post_url 2020-04-27-Transaction_Broker_v1.53.0 %}).
* Includes additional healthcare data in the callback from Transaction Broker.

#### Bug fixes
* Resolves an issue that prevented a callback when performing save-only operation on the hosted payment page (HPP). 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Wednesday, May 20th between 5:00 PM and 6:00 PM Pacific.
<br>
**Production**: Thursday, May 21st between 5:00 PM and 6:00 PM Pacific.
