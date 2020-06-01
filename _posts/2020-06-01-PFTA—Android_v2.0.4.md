---
layout: post
title: PFTA—Android v2.0.0
tag: PFTA-Android
author: AxiaMed
---
We've created the Payment Fusion Terminal Application to support the addition of PAX A80 and A920 devices to the Payment Fusion platform.

#### Features:

This initial release of the Payment Fusion Terminal Application for Android devices includes the following:
* Substantial UX uplift to deliver a superior patient payment experience
* The admin menu is now accessible using a standard password as opposed to a unique per terminal maintenance password in the earlier release. However select advanced menus still need per terminal unique maintenance password
* Tipping is now supported in the confirm transaction flow


#### Bug Fixes:

PFTA_Android_ReleaseNotes_2.0.3
* NFC transaction failing with Mastercard is fixed 
* NFC/tap now works with ApplePay/GooglePay 
* Wi-Fi configuration option from the admin menu for A80 is removed as we only support ethernet currently on this model
* NFC transaction failing with Mastercard is fixed
* NFC/tap now works with ApplePay/GooglePay
* Wi-Fi configuration option from the admin menu for A80 is removed as we only support ethernet currently on this model
* Transaction processing screen now reflects the transaction state more accurately
* A proper error message is displayed for an expired credit card
* A transaction with confirm_amount: true now displays the amount
* PFTA crash on an invalid transaction is now fixed
* A manual transaction now triggers Confirm_amount flow

&nbsp;  
###### Deployment schedule
* * *
**PFTA—Android for PAX A80** is available now in all environments
<br>
**PFTA—Android for PAX A920** is available now in all environments
