---
layout: post
title:  "X-XSS-Protection - Legacy Header"
date:   2021-05-15 19:25:00 +0530
categories: Security Updates
published:	true 
description: X-XSS-Protection header was used to prevent Cross-Site Scripting attack. This feature was mostly used in Internet Explorer, Chrome and Safari. X-XSS-Protection header restricted the execution of Reflected Cross-Site Scripting attacks. Currently, Chrome, Firefox and Edge no longer support the header "X-XSS-Protection". This also means that the applications which were only using "X-XSS-Protection" header are now unsafe from the Cross-Site Scripting.
browsers: Chrome 78+
downgrade: true
---

## Description 

The security feature by implementing the "X-XSS-Protection" header was used to prevent Cross-Site Scripting attack. This feature was mostly used in Internet Explorer, Chrome, Edge and Safari. X-XSS-Protection header restricted the execution of Reflected Cross-Site Scripting attacks. Nowadays, Content-Security-Policy is widespread and disables the use of inline JavaScript (‘unsafe-inline’) and eliminates the use of X-XSS-Protection header.

Currently, Chrome, Firefox and Edge no longer support the header "X-XSS-Protection". This also means that the applications which were only using the "X-XSS-Protection" header are now unsafe from Cross-Site Scripting. It is recommended to switch to the latest security features such as Content-Security-Policy to prevent Cross-Site Scripting exploitation.

## Browser(s)
* Chrome 78+

## Reference(s)
* [X-XSS-Protection](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection)
* [Chromium Bug Tracker](https://bugs.chromium.org/p/chromium/issues/detail?id=968591#c10)
* [Firefox never deployed X-XSS-Protection](https://bugzilla.mozilla.org/show_bug.cgi?id=528661)
* [MS Edge retired XSS Filter](https://blogs.windows.com/windows-insider/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/)
