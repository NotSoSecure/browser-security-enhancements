---
layout: post
title:  "Tabnabbing Protection"
date:   2021-05-10 18:25:06 +0530
categories: Security Updates
published:	true 
description: Reverse tabnabbing is an attack where an attacker can link a malicious page on the target application. The browsers recently added Tabnabbing protection and no longer allows access to the properties of "windows.opener". As browsers prevent Tabnabbing vulnerability and do not disclose "windows.opener" information to the opener page, this shows a NULL response. We can say that the browsers eliminated the Tabnabbing vulnerability by securing opener information Additionally, if you want to opt out from Tabnabbing prevention, the web pages can use rel="opener".
browsers: Chrome 88+
---

## Description 
Reverse tabnabbing is an attack where an attacker can link a malicious page on the target application. The browsers recently added Tabnabbing protection and no longer allows access to the properties of "windows.opener". As browsers prevent Tabnabbing vulnerability and do not disclose "windows.opener" information to the opener page, this shows a NULL response. We can say that the browsers eliminated the Tabnabbing vulnerability by securing opener information Additionally, if you want to opt out from Tabnabbing prevention, the web pages can use rel="opener".

## Browser(s) 
Chrome 88+

## Reference(s)
* [Anchor target=_blank implies rel=noopener by default](https://www.chromestatus.com/features/6140064063029248)