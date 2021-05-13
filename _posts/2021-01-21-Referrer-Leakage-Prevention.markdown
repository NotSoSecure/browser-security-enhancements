---
layout: post
title:  "Referrer Leakage Prevention"
date:   2021-05-10 18:26:06 +0530
categories: Security Updates
published:	true 
description: Referrer Policy is used to prevent referer header leakage. Chrome has changed a referrer policy defaults and is now using "strict-origin-when-cross-origin" as the default policy, instead of "no-referrer-when-downgrade". On cross-origin requests made from the web page without a referrer policy set on it, default configuration of Chrome will set "strict-origin-when-cross-origin" and prevent the Referer header leakage by disclosing initiating origin only instead of full URL.
browsers: Chrome 85+
---

## Description 
Referrer Policy is used to prevent referer header leakage. Chrome has changed a referrer policy defaults and is now using "strict-origin-when-cross-origin" as the default policy, instead of "no-referrer-when-downgrade". On cross-origin requests made from the web page without a referrer policy set on it, default configuration of Chrome will set "strict-origin-when-cross-origin" and prevent the Referer header leakage by disclosing initiating origin only instead of full URL.

## Browser(s) 
Chrome 85+

## Reference(s)
* 