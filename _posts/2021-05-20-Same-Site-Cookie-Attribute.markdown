---
layout: post
title:  "Same-Site Cookie Attribute"
date:   2021-05-20 13:15:00 +0530
categories: Security Updates
published:	true 
description: Same-Site attribute can be used to prevent Cross-Site Request Forgery attacks by asserting that the Browsers will not transmit the Same-Site cookie attribute if accessed from cross-origin which means we can prevent the Cross-Site Request Forgery attacks. Same-Site cookie attribute supports 3 values - Lax, Strict and None
Browser: Chrome 84+, Firefox 60+
---

## Description 
Same-Site attribute can be used to prevent Cross-Site Request Forgery attacks by asserting that the Browsers will not transmit the Same-Site cookie attribute if accessed from cross-origin which means we can prevent the Cross-Site Request Forgery attacks. 
Same-Site cookie attribute supports 3 values - Lax, Strict and None
* Lax: Cookies marked with Lax are not sent on the cross-site requests, i.e. load images or frames into a third party application
* Strict: cookies marked with Strict will only be sent on first requests and not being sent with the requests originating by third party applications.
* None: Cookies marked with None will not be sent to both first requests and cross-origin requests.

## Browser(s) 
Chrome 84+, Firefox 60+

## Reference(s)
* [Same-Site attribure](https://www.chromium.org/updates/same-site/test-debug)