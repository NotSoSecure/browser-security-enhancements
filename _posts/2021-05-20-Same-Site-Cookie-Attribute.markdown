---
layout: post
title:  "Same-Site Cookie Attribute"
date:   2021-05-21 13:15:00 +0530
categories: Security Updates
published:	true 
description: Same-Site attribute can be used to prevent Cross-Site Request Forgery attacks by asserting that the Browsers will not transmit the Same-Site cookie attribute if accessed from cross-origin which means we can prevent the Cross-Site Request Forgery attacks. Same-Site cookie attribute supports 3 values - Lax, Strict and None. The browsers consider Lax as the default value if Same-Site attribute is not present for the particular cookie. This will ensure that Cross-Site Request Forgery will not be allowed when an attacker attempts to execute it by request from an attacker controlled application.
browsers: Chrome 84+, Firefox 60+
---

## Description 
Same-Site attribute can be used to prevent Cross-Site Request Forgery attacks. Browsers will not transmit the Same-Site cookie attribute if access from cross-origin which means we can prevent the Cross-Site Request Forgery attacks. However, an attacker can still use Cross-Site Scripting vulnerability and perform chaining attack to execute Cross-Site Request Forgery attack.

We discussed how the Same-Site cookie attribute works. Now, let's understand it with respect to Chrome and Firefox browsers. Same-Site cookie attribute supports 3 values Lax, Strict and None:

* Lax: Same-Site cookies marked with Lax are not sent on the cross-site requests, i.e. load images or frames into a third party application. However, it is being sent when a user is navigating to the site by following a link from the application. 
* Strict: Same-Site cookies marked with Strict will only be sent on first requests and not being sent with the requests originating by third party applications. 
* None: Same-Site cookies marked with None will not be sent to both first requests and cross-origin requests. However, if the application sets Same-Site with None, it is required to set a Secure attribute which makes sure that cookie will not be transferred over an unencrypted HTTP channel. 

The browsers consider Lax as the default value if Same-Site attribute is not present for the particular cookie. This will ensure that Cross-Site Request Forgery will not be allowed when an attacker attempts to execute it by request from an attacker controlled application.

Following is the list of browsers which supports Same-Site attribute(as of 25 February 2021):
* Chrome 51, Some features are updated from Chrome 84
* Firefox 60
* Edge 16
* Opera 39
* Safari 13 on macOS 10.15 Catalina

## Browser(s) 
* Chrome 84+
* Firefox 60+

## Reference(s)
* [Same-Site attribure](https://www.chromium.org/updates/same-site/test-debug)