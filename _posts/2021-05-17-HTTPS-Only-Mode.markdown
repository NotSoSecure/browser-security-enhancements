---
layout: post
title:  "HTTPS-Only Mode"
date:   2021-05-17 16:20:06 +0530
categories: Security Updates
published:	true 
description: The HTTPS-Only mode restricts users from accessing HTTP applications, as it will not allow HTTP requests to pass through the browser. However, the web applications which only supports HTTP and the connection cannot be upgraded. If HTTPS-Only Mode is enabled and a HTTPS version of a site is not available, users will see a "Secure Connection Not Available" page which can be accessible after accepting the risk warning. HTTPS-Only Mode will be turned off temporarily for that site.
browsers: Firefox 83+
---

## Description 
The browser allows users to change the HTTPS-Only mode preferences. This is a security enhancement which restricts users from accessing HTTP applications in the case. However, there are a couple of caveats to discuss about this feature.

HTTPS-Only mode is a great security enhancement as it will not allow HTTP requests to pass through the browser, but what about the web applications which only supports HTTP and the connection cannot be upgraded. If HTTPS-Only Mode is enabled and a HTTPS version of a site is not available, users will see a "Secure Connection Not Available" page which can be accessible after accepting the risk warning. HTTPS-Only Mode will be turned off temporarily for that site. 

Anyway it can be self-understandable that if the application uses the "Strict-Transport-Security" header, the browsers do not allow the users to access HTTP applications. Security concerned web applications can always set "Strict-Transport-Security" which prevents requests to HTTP. To avoid the first request over HTTP while using "Strict-Transport-Security", the domains can be added to the preload list of web browsers. 


## Browser(s) 
* Firefox 83+

## Reference(s)
* [HTTPS-Only Mode](https://blog.mozilla.org/security/2020/11/17/firefox-83-introduces-https-only-mode/)