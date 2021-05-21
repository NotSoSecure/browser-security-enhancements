---
layout: post
title:  "X-XSS-Protection - Legacy Header"
date:   2021-05-19 19:25:00 +0530
categories: Security Updates
published:	true 
description: X-XSS-Protection header was used to prevent Cross-Site Scripting attack. This feature was mostly used in Internet Explorer, Chrome and Safari. X-XSS-Protection header restricted the execution of Reflected Cross-Site Scripting attacks. Currently, Chrome, Firefox and Edge no longer support the header “X-XSS-Protection”. This also means that the applications which were only using “X-XSS-Protection” header are now unsafe from the Cross-Site Scripting.
Browser: chrome 78+
---

## Description 
X-XSS-Protection header was used to prevent Cross-Site Scripting attack. This feature was mostly used in Internet Explorer, Chrome and Safari. X-XSS-Protection header restricted the execution of Reflected Cross-Site Scripting attacks. Currently, Chrome, Firefox and Edge no longer support the header “X-XSS-Protection”. This also means that the applications which were only using “X-XSS-Protection” header are now unsafe from the Cross-Site Scripting. Hence, It is recommended to switch to latest security features such as Content-Security-Policy to prevent Cross-Site Scripting exploitation which disables the use of inline JavaScript (‘unsafe-inline’) and eliminates the use of X-XSS-Protection header.

## Browser(s) 
chrome 78+

## Reference(s)
* [X-XSS-Protection](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection)