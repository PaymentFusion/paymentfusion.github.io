---
layout: post
title: Transaction Broker 2020.1.0
tag: Transaction Broker
author: AxiaMed
---

This release improves the status details from a terminal, and delivers performance and stability improvements.

**NOTE:** The versioning schema has been changed for our product releases. All product releases going forward will adopt a notation using the current year, release count, and hotfix. (e.g. 2020.1.0). This schema will provide release-cycle flexibility, and make it easier to interpret a product's release. 

#### New features
* Added details to **GET** `/terminals/{id}/status` and **GET** `/terminals/status` endpoints.  
    * Online / offline indicator
    * Busy indicator
    * The `tb_id` of an active job
    * Indicates if a card has been left inserted in the device
*  Status details have been added to the `"error_code": 4` response when sending a job to a busy terminal.

#### Bugs
* Fixes an issue where an error could be returned after a successful transaction void request. 

&nbsp;  
###### Deployment schedule
* * *
**Sandbox**: Monday, November 9 between 12:00 AM and 1:00 AM PDT
<br>
**Production**: Thursday, November 12 between 12:00 AM and 1:00 AM PDT
