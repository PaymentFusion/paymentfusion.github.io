---
layout: post
title: Settings API v1.13.0
tag: Settings API
author: AxiaMed
---
This update improves stability and resolves bugs for the hosted payment page (HPP) and terminal image handling. 

#### Bug fixes
* Resolves an issue where the background image was being improperly resized
* **GET** `/hpps` for a merchant without a configured HPP no longer returns `"error_message": "Unauthorized Access"`

#### Documentation
* HPP identifier now displays the type as "string"
* Adds additional error codes to a few endpoints:
  * **GET** `/hpps` → 4xx → 35, 36
  * **GET** `/sources` → 4xx → 34, 35, 36, 37
  * **GET** `/terminals` → 4xx → 34, 35, 36, 37


&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Tuesday, June 16 between 1:00 AM and 2:00 AM Pacific.
<br>
**Production**: Wednesday, June 17 between 12:00 AM and 1:00 AM Pacific.
