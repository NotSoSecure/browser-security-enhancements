---
layout: post
title:  "Total Cookie protection in Firefox"
date:   2021-05-20 11:45:20 +0530
categories: Security Updates
published:	true 
description: Total Cookie Protection creates a separate "cookie jar" for each website the users visit in Firefox. Any time a website, or third-party content embedded in a website, deposits a cookie in your browser, that cookie is confined to the cookie jar assigned to that website, such that it is not allowed to be shared with any other website.
browsers: Firefox 86+
---

## Description 
Total Cookie Protection creates a separate "cookie jar" for each website the users visit in Firefox. Any time a website, or third-party content embedded in a website, deposits a cookie in your browser, that cookie is confined to the cookie jar assigned to that website, such that it is not allowed to be shared with any other website. For example, if the user accesses the website "www.notsosecure.com", and it contains third party contents from "api.thirdpartycontents.com". The browser will create a "cookie jar" and store both cookies "www.notsosecure.com" and "api.thirdpartycontents.com" to the "cookie jar" of "www.notsosecure.com" - the first web application which users accessed. If the user accesses another application which uses any of the above applications, the browser will not use the cookie and create a new cookie jar for each application the user visits. 

How will this affect normal users? The applications which support Sign in with Google, Facebook or any other applications will not allow to access the applications directly with the existing cookies. Instead of this, the applications will ask users to sign again to their provider and use the cookies separately. 

Addtionally, Enhanced Tracking Protection is the default setting for Firefox users and will block the following trackers:
* Cross-site cookies
* Social media trackers
* Cryptominers
* Tracking content in private windows
* Fingerprinters

## Browser(s) 
* Firefox 86+

## Reference(s)
* [Total Cookie Protection in Firefox](https://blog.mozilla.org/security/2021/02/23/total-cookie-protection/)