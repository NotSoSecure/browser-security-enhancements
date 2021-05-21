---
layout: post
title:  "Tabnabbing Protection"
date:   2021-05-19 18:25:06 +0530
categories: Security Updates
published:	true 
description: Reverse tabnabbing is an attack where an attacker can link a malicious page on the target application. The browsers recently added Tabnabbing protection and no longer allows access to the properties of "windows.opener". As browsers prevent Tabnabbing vulnerability and do not disclose "windows.opener" information to the opener page, this shows a NULL response. We can say that the browsers eliminated the Tabnabbing vulnerability by securing opener information Additionally, if you want to opt out from Tabnabbing prevention, the web pages can use rel="opener".
browsers: Chrome 88+
---

## Description 
Reverse tabnabbing is an attack where an attacker can link a malicious page on the target application. The malicious page is able to rewrite the target application, for example to replace it with a phishing site. As the user was originally on the correct page they are less likely to notice that it has been changed with a phishing site, especially if the site looks the same as the target. If the user authenticates to this phishing site then their credentials (or other sensitive data) are sent to the phishing site rather than the legitimate one.

The following list of properties can be accessed by a malicious application:
* opener.closed: Returns a boolean value indicating whether a window has been closed or not.
* opener.frames: Returns all iframe elements in the current window.
* opener.length: Returns the number of iframe elements in the current window.
* opener.opener: Returns a reference to the window that created the window.
* opener.parent: Returns the parent window of the current window.
* opener.self: Returns the current window.
* opener.top: Returns the topmost browser window.

However, the browsers recently added Tabnabbing protection and no longer allows access to the properties mentioned above. To prove it let’s see an example mentioned below:

<a target="_blank" href="https://attacker.com">Click Here! </a>

As browsers prevent Tabnabbing vulnerability and do not disclose “windows.opener” information to opener page, this shows a NULL response. 

So, we can say that the browsers eliminated the Tabnabbing vulnerability by securing opener information. 
Additionally, if you want to opt out from Tabnabbing prevention, the web pages can use rel="opener" as shown below:

<a target="_blank" href="https://notsosecure.com" rel="opener">Click!</a>

## Browser(s) 
* Chrome 88+

## Reference(s)
* [Anchor target=_blank implies rel=noopener by default](https://www.chromestatus.com/features/6140064063029248)
* [HTML Updates - Following hyperlinks](https://html.spec.whatwg.org/#following-hyperlinks)